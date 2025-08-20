% movement, kerberos, asreproast, impacket

# 通过ASREProast进行用户名枚举
```sh
impacket-GetNPUsers $DOMAIN/ -usersfile usernames_todo.txt | grep -v "Client not found in Kerberos database"
```