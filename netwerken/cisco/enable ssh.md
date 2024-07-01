 #cisco #setup 
1. enter global config 
```bash 
conf t
```
2. conf ip domain 
```bash
ip domain name 'name'
```
3. genereer encryption 
```bash
crypto key generate rsa general-keys modulus 1024
```
4. maak een local user 
```bash 
username 'user' secret 'wachtwoord'
```
5. enter vty ports
```bash
line vty 0 4
```
6. authentiseer op local database 
```bash 
login local 
```
7. transport aangeven 
```bash
transport input ssh
```
8. exit 
```bash 
exit
```



- verify 
```bash
ssh user@serverip
```
