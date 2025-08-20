% init, child

# 为凭据单独创建目录，初始化环境变量
```sh
mkdir <child_name>
echo source_up >> <child_name>/.envrc
echo export USER= >> <child_name>/.envrc
echo export PASSWORD= >> <child_name>/.envrc

echo "环境初始化完毕，收集到新的信息时，请编辑 .envrc 文件"
echo "收集到新凭据时，使用 init, child 创建一个单独的工作目录"
direnv allow <child_name>
```
