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
