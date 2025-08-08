% init, main

# 创建靶场目录，初始化环境变量，每个凭据都需要一个单独的目录
```sh
mkdir <main_name>
cd <main_name>
echo export MACHINE_IP=<machine_ip> > .envrc
echo export DOMAIN=       >> .envrc
echo export DC_IP=        >> .envrc
echo export DC_HOST=      >> .envrc
echo export USER=         >> .envrc
echo export PASSWORD=     >> .envrc
echo "username, password" > user-pass.csv
echo "username, ntlmhash" > user-hash.csv

direnv allow .

echo "环境初始化完毕，收集到新的信息时，请编辑 .envrc 文件"z
echo "收集到新凭据时，使用 init, child 创建一个单独的工作目录"
echo "当前目标: <machine_ip>"
```
