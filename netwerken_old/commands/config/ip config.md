#config #ip 
### ip interfaces 
**Omschrijving**: Toont de IP-statistieken voor alle interfaces op een router.
1. IPv4
```vim 
show ip interface
```
2. Ipv6 
```vim 
show ipv6 interface
```
### ip interfaces vrief
**Omschrijving** : De uitvoer toont alle interfaces, hun IP-adressen en hun huidige status. De geconfigureerde en verbonden interfaces moeten een status van “up” en een protocol van “up” weergeven. Al het andere zou duiden op een probleem met de configuratie of de bekabeling.
1. ip 
```vim
show ip interface brief 
```
2. IPv6 
```vim
show ipv6 interface brief
```
## ip route
**Omschrijving**: Toont de inhoud van de IP-routeringstabellen die zijn opgeslagen in RAM.
1. IPv4
```vim 
show ip route 
```
2. IPv6 
```vim 
show ipv6 route 
```
