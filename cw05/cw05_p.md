## h 5.1 p
```bash
wget https://github.com/opsec-infosec/nmap-static-binaries/releases/download/v2/nmap-x64.tar.gz
scp nmap-x64.tar.gz student@192.168.100.105:/home/student
ssh student@192.168.100.105 #Password: pjatk
tar zxvf nmap-x64.tar.gz
```

## h 5.2 p
```bash
#Replace TARGET_IP with the IP from homework [H]
./nmap -n -Pn -sV -p- -vv TARGET_IP
```
