## h 9.1 p
```bash
#Kali:
hashcat -m 0 498c9984309d201da4ad7f354b5ce5d0 /usr/share/wordlists/rockyou.txt
```

> **Answer:** `oncyqyu`

## h 9.2 p
```bash
#Kali:
hashcat -m 100 afd769dda3bb68338650b0cfccb147e9d13d8217 /usr/share/wordlists/rockyou.txt
```

> **Answer:** `KAMEHAME`

## h 9.3 p
```bash
#Kali:
hashcat -S -m 3200 '$2a$12$GZcp1ScNwZ762Vtb/6sbOOsUz1RzBuwUofk8jx9Ahv8ASi15PzL6u' /usr/share/seclists/Passwords/Leaked-Databases/rockyou-75.txt
```

> **Answer:** `scarlett1`

## h 9.4 p
```bash
#Kali:
hashcat -m 1000 B8DBB1B31B974AC88A49A4FF1E885BA4 -a3 ?d?d?d?d?d?d?d?d?d
```

> **Answer:** `758741256`

## h 9.5 p
```bash
#Kali - download Plik.zip from the platform:
zip2john Plik.zip > hash5_p
john --wordlist=/usr/share/wordlists/rockyou.txt hash5_p
unzip Plik.zip #Password: obvious
cat flag.txt
```

> **Answer:** `PJATK{TooObvious}`
