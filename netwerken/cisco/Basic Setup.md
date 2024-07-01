#setup #cisco 

1. Enter global Configuration Mode 
```bash
configure terminal 
```
2. Set Hostname 
```bash 
hostname 'host'
```
- verify 
```bash 
show running-config | include hostname 
```
3. set banner 
```bash 
banner motd # banner # 
```
4. secure privileged mode 
```bash
enable password 'wachtwoord'
```
5. secure user Exec Mode
```bash
line console 0

login 'wachtwoord'

end 
```
6. Encrypt password 
```bash 
service password-encryption
```



