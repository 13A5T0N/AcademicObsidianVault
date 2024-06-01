1. Access privileged mode 
```vim
configure terminal
```
2. *Setup hostname*
```vim 
hostname 'name'
```
3. configureer ip domain 
```vim 
ip domain name "domain"
```
4. genereer een encryption key voor ssh 
```vim 
crypto key generate rsa general-keys modulus 1024
```
6. controleer of maak een local gebruiker 
```vim 
username "user" secret "wachtwoord" 
```
7. enable vty ports 
```vim 
line vty 0 4 
```
8. authtentiseer op local database
```vim 
login local
```
9. transport aangeven
```vim 
transport input ssh
```
10. exit 
```vim
exit
```
