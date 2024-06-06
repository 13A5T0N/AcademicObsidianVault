#secure #config

1. enter globale config mode 
``` vim 
configure terminal
```
2.   enter line vty config 
``` vim 
line vty 0 15
```
3. wachtwoord aangeven 
```vim
password 'wachtwoord'
```
4. enable vty toegang
```vim 
login
```
5. eruit gaan
```vim 
end
```

**Note**: meeste **Cisco switches** hebben 16 vty lines genummerd van 0 - 15 
