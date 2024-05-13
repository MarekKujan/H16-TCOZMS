a)
1. Vysvetlite význam a opodstatnenie IP adries
   - umožňujú nám adresovanie na globálnej úrovni
2. Definujte triedy IP adries v IPv4
   - triedy su legacy met=oda triedenia IP adries
   - poznáme triedy: A, B, C, D, E
   - Trieda A
     - maska 255.0.0.0
     - verejné IP adresy: 1.0.0.0 - 127.0.0.0
     - privátne IP adresy: 10.0.0.0 - 10.255.255.255
     - počet hostov: 16,777,214
   - Trieda B
     - maska 255.255.0.0
     - verejné IP adresy: 128.0.0.0 - 191.255.0.0
     - privátne IP adresy: 172.16.0.0 - 172.31.255.255
     - počet hostov: 65,534
   - Trieda C
     - maska 255.255.255.0
     - verejné IP adresy: 192.0.0.0 to 223.255.255.0
     - privátne IP adresy: 192.168.0.0 to 192.168.255.255
     - počet hostov: 254
   - Trieda D
     - multicast adresy
   - Trieda E
     - špeciálne adresy
3. Popíšte význam masky v IPv4
   - rozdeľuje a udáva hostovskú a sieťovú časť IP adresy
   - sieťová adresa môže obsahovať bity 1 len v sieťovej časti adresy
   - na binárnej úrovni maska -> každý bit vyznačený 1 patrí sieti a ostatné patria hostovi
4. Zdôvodnite potrebu broadcastovej adresy
   - broadcastová adresa môže slúžiť na informácie, ktoré potrebuje sieť doručiť každému užívateľovi
   - patria sem najmä ARP, IPV6 router advertisement
   - efektívne pri spojení sa so zariadeniami, ktoré ešte nepoznáme
5. Analyzujte potrebu vzniku IPv6
   - vyčerpanie IPv4 adries
   - vnziká potreba rozdelenia sietí na privátne a verejné
   - koncové zariadenia nie sú globálne routovatelné, skoro každá sieť využíva NAT
   - IPv6 vytvorená s priestorom na dostatočne množstvo zariadení
   - každý počítač môže byť globálne routovatelní
b)
1. Určte možnosti podsieťovania, ak je dĺžka prefixu /24
   - tretí oktet je voľný? 255 podsietí?
   - VLSM, ak máme priradenú jednú /24 sieť môžeme si ju rozdeliť na menšie aby sme zachovali IP adresy
2. Popíšte vlastnosti IP protokolu
   - adresovanie počítačov
   - nezávislosť na médiu
   - smerovanie paketov
   - best effort
1. Porovnajte hlavičky paketu IPv4 a IPv6, použite obrazovú prílohu č. 8
   - mate tam obrazok tak asi vam to pojde
c)
1. Popíšte rôzne formy platobného styku (elektronické bankovníctvo)
2. Vysvetlite spôsob vykonania príkazu priradenia, uveďte príklad
