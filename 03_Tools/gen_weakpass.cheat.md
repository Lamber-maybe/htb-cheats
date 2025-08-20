% weakpass

# 生成弱密码字典, 规则: 用户名大小写
```sh

> user.txt
> pass.txt

while read u; do
  echo "$u"       >> user.txt
  echo "$u"       >> pass.txt

  echo "$u"       >> user.txt
  echo "${u^^}"   >> pass.txt

  echo "$u"       >> user.txt
  echo "${u,,}"   >> pass.txt
done < users.txt
```
