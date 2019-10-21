# Usage

smbexec.exe -h HOST_IP -u user -p password -e command

```
smbexec.exe -h 192.168.111.1 -u user -p 123456 -e "cmd.exe /c start calc.exe "
```

# Description

This exe will allow you to execute a command on a target machine using SMB by user&password.

smbexec.exe  will oputput "execserver.exe" to the folder \\host\admin$, and create a remote service.

When the remote service started, smbexec.exe send the command to remote service by open pipe: \\Host_IP\pipe\\SMBEXEC


# Build & Test

1. Open smbexec.sln by VC2010SP1, Build sulotion
2. Test On Win7 + 2018 Server in VM



