a)
1. Charakterizujte význam binárneho číselného kódu vo výpočtovej technike
2. Porovnajte kombinačné a sekvenčné logické obvody
3. Porovnajte pravdivostné tabuľky dvojvstupových logických obvodov AND, NAND, OR a NOR
4. Objasnite rozdiel medzi monostabilným (M.K.O.), bistabilným (B.K.O.) a astabilným klopným obvodom (A.K.O.)
5. Vysvetlite a popíšte reprodukčný proces podniku, jeho vstupy a výstupy
b)
1. Definujte hexadecimálnu sústavu
2. Načrtnite využitie hexadecimálneho kódu v počítačových sieťach
3. Charakterizujte binárnu číselnú sústavu a jej využitie v praxi
c)
1. Zvoľte si a vyjadrite v binárnom kóde IPv4 adresu s dĺžkou prefixu 24
2. Porovnajte IPv4 siete a IPv4 hosta

---
##### Charakterizujte význam binárneho číselného kódu vo výpočtovej technike
- Binárny číselný kód je systém reprezentácie čísel, kde sa používajú len dve cifry - 0 a 1. Cifra v binárnom kóde sa nazýva bit (z anglického binary digit).
- Binárny kód je základným stavebným blokom pre digitálne systémy a je často používaný v počítačoch a elektronike na reprezentáciu čísel, znakov, obrázkov a iných dátových typov.
- Pán Bool (George Boole), matematik a logik, v 19. storočí vyvinul Booleovu algebru. Táto algebra je základom pre digitálne obvody a logické operácie.
- Napäťové stavy sa používajú v elektronike na reprezentáciu binárneho kódu.
##### porovnajte kombinačné a sekvenčné logické obvody
**Kombinačné logické obvody**:
- Kombinačné logické obvody sú závislé iba od aktuálnych vstupných hodnôt a nemajú žiadnu pamäťovú funkciu.
- Výstupné hodnoty kombinačných obvodov sú určené výlučne kombináciou vstupných hodnôt a logických operácií, ktoré sa na ne aplikujú.
- Príklady kombinačných obvodov zahŕňajú logické brány (AND, OR, NOT), multiplexéry, demultiplexéry.
**Sekvenčné logické obvody**:
- Sekvenčné logické obvody majú pamäťovú funkciu a ich výstupné hodnoty závisia nielen od aktuálnych vstupných hodnôt, ale aj od stavu pamäte.
- Pamäťový stav sa mení na základe vstupných hodnôt a vnútorného stavu obvodu.
- Príklady sekvenčných obvodov zahŕňajú TON, TOFF, registre, klopé obvody.
- Sekvenčné obvody sú vhodné pre zložitejšie operácie, ktoré vyžadujú uchovávanie stavu a riadenie postupnosti udalostí.
**Porovnanie**:
- **Časová závislosť:** Kombinačné obvody nemajú vnútorný stav a generujú výstup okamžite, zatiaľ čo sekvenčné obvody majú pamäť a ich výstup závisí aj od predchádzajúceho stavu.
- **Pamäťové prvky:** Kombinačné obvody nemajú pamäťové prvky, zatiaľ čo sekvenčné obvody ich majú a môžu uchovávať informácie medzi jednotlivými vstupmi.
##### Porovnajte pravdivostné tabuľky dvojvstupových logických obvodov AND, NAND, OR a NOR
![[log_obvody.png]]
##### Objasnite rozdiel medzi monostabilným (M.K.O.), bistabilným (B.K.O.) a astabilným klopným obvodom (A.K.O.)
**Monostabilný klopný obvod:**
- Charakteristika: Má jediný stabilný stav. Po prijatí vstupného signálu vstúpi do nestabilného stavu počas určitého času (označovaného ako časová konštanta), po ktorom sa vráti do svojho stabilného stavu.
- Využitie: Generovanie krátkych impulzových signálov alebo oneskorení.
**Bistabilný klopný obvod:**
- Charakteristika: Má dva stabilné stavy a môže zostať v ktoromkoľvek z nich aj po zmene vstupných podmienok. Nie je závislý na časových konštantách a zostane v aktuálnom stave, kým nedostane inštrukciu na zmenu.
- Využitie: Používa sa na uchovávanie pamäte alebo na realizáciu spínačov a prepínačov.
**Astabilný klopný obvod:**
- Charakteristika: Nemá stabilný stav. Neustále mení svoj stav medzi dvoma rôznymi hodnotami v pravidelných intervaloch, čo vytvára periodický signál.
- Využitie: Používa sa na generovanie oscilačných signálov, ako sú kvapalné hodiny, blikajúce svetlá alebo generátory pulzov.
##### [[EKN#Vysvetlite a popíšte reprodukčný proces podniku, jeho vstupy a výstupy]]
##### definujte hexadecimálnu sústavu
- číselný systém,  používa 16 symbolov na reprezentáciu čísel. Tieto symboly sú číslice od 0 do 9 a písmená od A do F, pričom A reprezentuje hodnotu 10, B hodnotu 11 a tak ďalej, až po F, ktoré reprezentuje hodnotu 15.
- V hexadecimálnej sústave sa každá číslica váži podľa mocniny čísla 16.
- Hexadecimálna sústava je často používaná v počítačovej vede a programovaní, pretože je veľmi vhodná na reprezentáciu binárnych čísel. Každému štvorbitovému binárnemu číslu (4 bity) zodpovedá jedna hexadecimálna číslica.
##### načrtnite využitie hexadecimálneho kódu v počítačových sieťach
- IPv6 adresy sú dlhšie a zložitejšie ako IPv4 adresy a sú zvyčajne zapisované v hexadecimálnej sústave. IPv6 adresa je 128-bitové číslo, ktoré je rozdelené do 8 skupín po 4 hexadecimálnych číslach. Každá skupina je oddelená dvojbodkou. Napríklad, 2001:0db8:85a3:0000:0000:8a2e:0370:7334 je jedna z možných IPv6 adries.
- MAC adresy, ktoré slúžia na jednoznačnú identifikáciu sieťových zariadení, sú tiež zvyčajne zapisované v hexadecimálnej sústave. MAC adresa je 48-bitové číslo, ktoré je rozdelené do 6 skupín po 2 hexadecimálnych číslach. Každá skupina je oddelená dvojbodkou. Napríklad, 00:1A:2B:3C:4D:5E je jedna z možných MAC adries.
##### charakterizujte binárnu číselnú sústavu a jej využitie v praxi
Binárna číselná sústava je základným spôsobom reprezentácie čísel v počítačoch. V tejto sústave sa používajú len dve číslice - 0 a 1. Každá pozícia v čísle predstavuje mocninu čísla 2.
Binárna sústava je dôležitá v počítačoch, pretože počítače pracujú s elektrickými signálmi, ktoré môžu byť buď v stave zapnutia (1) alebo vypnutia (0). Vďaka binárnej sústave môžeme reprezentovať a manipulovať s číslami a dátami v počítačoch.
V elektronických obvodoch sa používajú logické brány a klopné obvody, ktoré pracujú s binárnymi signálmi. Binárna sústava je základom pre návrh a implementáciu digitálnych obvodov.
##### Zvoľte si a vyjadrite v binárnom kóde IPv4 adresu s prefixom 24
```
192.168.1.0/24
11000000.10101000.00000001.00000000/24
```
##### Porovnajte IPv4 siete a IPv4 hosta
- IP adresa siete nemá žiadné bity 1 v hostovskej časti
- IP hosťa má bity 1 v hostovskej časti, preto vieme že je to hostovská IP adresa