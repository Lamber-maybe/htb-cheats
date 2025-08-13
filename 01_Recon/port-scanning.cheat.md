% recon, port-scanning, rustscan

# 使用 rustscan 进行端口扫描[step_1，扫描完端口之后，如果有445开放则进行smb扫描]
```sh
rustscan -u 5000 -a $MACHINE_IP

echo "scan done, if 445, scan smb"
```

