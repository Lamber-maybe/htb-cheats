% recon, smb-scanning, netexec, Guest

# netexec 使用 Guest 账户枚举SMB服务
```sh
netexec smb $MACHINE_IP -u "Guest" -p "" --shares
```

% recon, smb-scanning, netexec, Anonymous

# netexec 使用 匿名 账户枚举SMB服务
```sh
netexec smb $MACHINE_IP -u "" -p "" --shares
```

% recon, smb-scanning, netexec, creds

# netexec 使用 当前 账户枚举SMB服务
```sh
netexec smb $MACHINE_IP -u "$USER" -p "$PASSWORD" --shares
```