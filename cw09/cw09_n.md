## 9.1
```bash
#Decode KQZGP{GlWlkrvilKlxazgvp} using an online Atbash decoder
#Submit the decoded flag on the platform
```

> **Answer:** `PJATKToDopieroPoczatek`

## 9.2
```bash
#Decode 50 4A 41 54 4B 7B 73 7A 65 73 6E 61 73 63 69 65 7D using an online HEX to text decoder
#Submit the decoded flag on the platform
```

> **Answer:** `PJATK{szesnascie}`

## 9.3
```bash
#Decode decimal ASCII codes using an online ASCII converter (decimal to text):
#80 74 65 84 75 123 116 64 98 101 108 64 122 110 97 75 111 119 125
#Submit the decoded flag on the platform
```

> **Answer:** `PJATK{t@bel@znaKow}`

## 9.4
```bash
#Decode UEpBVEt7YTExeW91cmJhc2V9 using an online Base64 decoder
#Submit the decoded flag on the platform
```

> **Answer:** `PJATK{a11yourbase}`

## 9.5
```bash
cat hex.bin
xxd hex.bin
```

## 9.6
```bash
#Calculate the MD5 hash of PJATK using an online MD5 generator
#Submit the hash on the platform
```

> **Answer:** `2777ad335d49b6759ed58b87c220dfde`

## 9.7
```bash
#Look up 3062e1e11c64939824f4f249890f7157 in an online MD5 hash database (e.g. md5decrypt.net)
#Submit the found plaintext in the format PJATK{flag}
```

> **Answer:** `PJATK{md5md5}`

## 9.8
```bash
#CyberChef (https://gchq.github.io/CyberChef/):
#Paste the HEX string from the task into Input
#From Hex -> Delimiter: Space
#XOR Brute Force -> Key length: 1, Sample length: 100, Sample offset: 0, Print key: enabled
#Find the readable flag (Key = 58 HEX)
```

> **Answer:** `PJATK{xorniejestbezpieczny}`

## 9.9
```bash
ssh student@192.168.100.9
openssl aes-256-cbc -pbkdf2 -d -in plik_enc_aes-256-cbc.bin #Password: PJATK
```

> **Answer:** `PJATK{Sym3tr1a}`
