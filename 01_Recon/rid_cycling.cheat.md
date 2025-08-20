% recon, 445-smb, rid cycling, netexec

# RID爆破, netexec
```sh
netexec smb $MACHINE_IP -u "${USER:-}" -p "${PASSWORD:-}" --rid-brute
```
