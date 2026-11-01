## h 5.1 p
```bash
#On Kali:
wget https://github.com/opsec-infosec/nmap-static-binaries/releases/download/v2/nmap-x64.tar.gz
scp nmap-x64.tar.gz student@192.168.100.5:/home/student/
#If SCP says 'No route to host', check VPN/machine and retry
ssh student@192.168.100.5 #Password: pjatk
#On the remote machine:
tar zxvf nmap-x64.tar.gz
```
