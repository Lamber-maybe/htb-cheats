% recon, 445-smb, shares, netexec, Guest

# netexec 使用 Guest 账户枚举SMB服务
```sh
netexec smb $MACHINE_IP -u "Guest" -p "" --shares
```

% recon, 445-smb, shares, netexec, Anonymous

# netexec 使用 匿名 账户枚举SMB服务
```sh
netexec smb $MACHINE_IP -u "" -p "" --shares
```

% recon, 445-smb, shares, netexec, creds

# netexec 使用 当前 账户枚举SMB服务
```sh
netexec smb $MACHINE_IP -u ${USER:-} -p ${PASSWORD:-} --shares
```

% recon, 1433-mssql, netexec, creds

# netexec 使用 当前 账户枚举MSSQL服务
```sh
netexec mssql $MACHINE_IP -u ${USER:-} -p ${PASSWORD:-}
```

% recon, 445-smb, shares, netexec, brute-creds

# netexec 使用 字典 爆破用户名密码(先设置user.txt和pass.txt到环境变量)
```sh
netexec smb $MACHINE_IP -u ${USER:-} -p ${PASSWORD:-} --no-bruteforce --continue-on-success --shares
```
