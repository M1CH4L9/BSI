## h 2.1 p
```bash
nmap -sT -sV -sC -O --osscan-guess -p- -vv 192.168.200.152
```

## h 2.2 p
```bash
curl http://192.168.200.152:8080/flag2.2p.txt
[ANSWER]
#BTW zmiany porty w curlu nie było na prezentacji itp. :))
```

## h 2.3 p
```bash
ftp 192.168.200.152
name: anonymous
password: [TYPE_ANYTHING]
get flag2.3p.txt
exit
cat flag2.3p.txt
[ANSWER]
#Type flag on website
```

## h 2.4 p
```bash
smbclient -N //192.168.200.152/FLAG
get flag2.4p.txt
exit
cat flag2.4p.txt
[ANSWER]
#Type flag on website
```
