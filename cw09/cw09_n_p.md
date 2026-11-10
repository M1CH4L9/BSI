## 9.1 p
```bash
#Kali - only if Hashcat has no OpenCL runtime:
sudo apt install pocl-opencl-icd clinfo

#Only if rockyou.txt is compressed:
sudo gunzip /usr/share/wordlists/rockyou.txt.gz

scp student@192.168.100.9:/home/student/hash1 ./
hashcat -m 0 hash1 /usr/share/wordlists/rockyou.txt
```

> **Answer:** `abc123`

## 9.2 p
```bash
#Kali:
scp student@192.168.100.9:/home/student/hash2 ./
hashcat -m 100 hash2 /usr/share/wordlists/rockyou.txt
```

> **Answer:** `AOM201`

## 9.3 p
```bash
#Kali:
scp student@192.168.100.9:/home/student/hash3 ./
hashcat -m 3200 hash3 /usr/share/wordlists/rockyou.txt
```

> **Answer:** `garfield`

## 9.4 p
```bash
#Kali:
scp student@192.168.100.9:/home/student/hash4 ./
hashcat -m 1000 hash4 -a3 ?d?d?d?d?d?d?d?d?d?d?d
```

> **Answer:** `35821259632`

## 9.5 p
```bash
#Kali:
scp student@192.168.100.9:/home/student/pkzip.zip ./
zip2john pkzip.zip > hash5
john --wordlist=/usr/share/wordlists/rockyou.txt hash5
unzip pkzip.zip #Password: Rynolds7
cat flag.txt
```

> **Answer:** `PJATK{Cr@ck_th3_@rchiv3}`

## 9.6 p
```bash
#Kali:
scp student@192.168.100.9:/home/student/file.rar ./
crunch 1 3 -f /usr/share/crunch/charset.lst lalpha-numeric > new_dict.txt
rar2john file.rar > hash6
john --wordlist=new_dict.txt hash6
unrar e file.rar #Password: dhh
strings file
```

> **Answer:** `PJATK{Strings_a0c4153}`
