---
share: "true"
---
## A
 - charakterizujte binárny číselný kód
 - načrtnite schematické značky logických členov AND, NOR, NOT
 - napíšte tabuľku pravdivostných hodnôt pre AND, NOR, NOT
 - definujte hexadecimálnu sústavu
 - `Ekonomická otázka` 
## B
- načrtnite využitie hexadecimálneho kódu v počítačových sieťach
- charakterizujte binárnu číselnú sústavu a jej využitie v praxi
- porovnajte kombinačné a sekvenčné logické obvody
## C
- Zvoľte si a vyjadrite v binárnom kóde IPv4 adresu s prefixom 24
- Porovnajte IPv4 siete a IPv4 hosta

---
##### charakterizujte binárny číselný kód
Binárny číselný kód je systém reprezentácie čísel pomocou dvojkového číselného systému, kde sa používajú len dve cifry - 0 a 1. Každá cifra v binárnom kóde sa nazýva bit (z anglického binary digit).
V binárnom kóde sa každé číslo vyjadruje pomocou kombinácie bitov. Napríklad, ak máme 8-bitový binárny kód, môžeme vyjadriť čísla od 0 do 255 (2^8 - 1).
Binárny kód je základným stavebným blokom pre digitálne systémy a je často používaný v počítačoch a elektronike na reprezentáciu čísel, znakov, obrázkov a iných dátových typov.
Pán Bool, známy ako George Boole, bol matematik a logik, ktorý v 19. storočí vyvinul Booleovu algebru. Táto algebra je základom pre digitálne obvody a logické operácie, ktoré sú základom pre binárny kód a digitálne systémy.
Napäťové stavy sú rôzne úrovne napätia, ktoré sa používajú v elektronike na reprezentáciu binárneho kódu. V digitálnych systémoch sa často používajú dva napäťové stavy - vysoký (1) a nízky (0). Tieto napäťové stavy sa používajú na reprezentáciu bitov v binárnom kóde.
##### načrtnite schematické značky logických členov AND, NOR, NOT + napíšte tabuľku pravdivostných hodnôt pre AND, NOR, NOT
![[log_obvody.png]]
##### definujte hexadecimálnu sústavu
Hexadecimálna sústava je číselný systém, ktorý používa 16 symbolov na reprezentáciu čísel. Tieto symboly sú číslice od 0 do 9 a písmená od A do F, pričom A reprezentuje hodnotu 10, B hodnotu 11 a tak ďalej, až po F, ktoré reprezentuje hodnotu 15.
V hexadecimálnej sústave sa každá číslica váži podľa mocniny čísla 16. Napríklad, číslo 10 v hexadecimálnej sústave je ekvivalentné číslu 16 v desiatkovej sústave, číslo 100 je ekvivalentné číslu 256 a tak ďalej.
Hexadecimálna sústava je často používaná v počítačovej vede a programovaní, pretože je veľmi vhodná na reprezentáciu binárnych čísel. Každému štvorbitovému binárnemu číslu (4 bity) zodpovedá jedna hexadecimálna číslica.
##### načrtnite využitie hexadecimálneho kódu v počítačových sieťach
IPv6 adresy sú dlhšie a zložitejšie ako IPv4 adresy a sú zvyčajne zapisované v hexadecimálnej sústave. IPv6 adresa je 128-bitové číslo, ktoré je rozdelené do 8 skupín po 4 hexadecimálnych číslach. Každá skupina je oddelená dvojbodkou. Napríklad, 2001:0db8:85a3:0000:0000:8a2e:0370:7334 je jedna z možných IPv6 adries.
MAC adresy, ktoré slúžia na jednoznačnú identifikáciu sieťových zariadení, sú tiež zvyčajne zapisované v hexadecimálnej sústave. MAC adresa je 48-bitové číslo, ktoré je rozdelené do 6 skupín po 2 hexadecimálnych číslach. Každá skupina je oddelená dvojbodkou. Napríklad, 00:1A:2B:3C:4D:5E je jedna z možných MAC adries.
Hexadecimálny kód je v týchto prípadoch výhodný, pretože umožňuje kompaktný a jednoduchý zápis týchto dlhých číselných hodnôt. Taktiež je jednoduché prevádzať medzi hexadecimálnou a binárnou sústavou, čo je dôležité pri práci s týmito adresami a identifikátormi v počítačových sieťach.
##### charakterizujte binárnu číselnú sústavu a jej využitie v praxi
Binárna číselná sústava je základným spôsobom reprezentácie čísel v počítačoch. V tejto sústave sa používajú len dve číslice - 0 a 1. Každá pozícia v čísle predstavuje mocninu čísla 2.
Binárna sústava je dôležitá v počítačoch, pretože počítače pracujú s elektrickými signálmi, ktoré môžu byť buď v stave zapnutia (1) alebo vypnutia (0). Vďaka binárnej sústave môžeme reprezentovať a manipulovať s číslami a dátami v počítačoch.
V elektronických obvodoch sa používajú logické brány a klopné obvody, ktoré pracujú s binárnymi signálmi. Binárna sústava je základom pre návrh a implementáciu digitálnych obvodov.
##### porovnajte kombinačné a sekvenčné logické obvody
Kombinačné logické obvody:
- Kombinačné logické obvody sú závislé iba od aktuálnych vstupných hodnôt a nemajú žiadnu pamäťovú funkciu.
- Výstupné hodnoty kombinačných obvodov sú určené výlučne kombináciou vstupných hodnôt a logických operácií, ktoré sa na ne aplikujú.
- Príklady kombinačných obvodov zahŕňajú logické brány (AND, OR, NOT), multiplexéry, demultiplexéry.
Sekvenčné logické obvody:
- Sekvenčné logické obvody majú pamäťovú funkciu a ich výstupné hodnoty závisia nielen od aktuálnych vstupných hodnôt, ale aj od stavu pamäte.
- Pamäťový stav sa mení na základe vstupných hodnôt a vnútorného stavu obvodu.
- Príklady sekvenčných obvodov zahŕňajú TON, TOFF, registre, klopé obvody (Monostabilný `za určitý čas sa po tom ako dostane sgnál sa vypne`, Astabilný `signalom sa zapne a vypne`, Bistabilný `začne kmitať keď dostane signál`).
- Sekvenčné obvody sú vhodné pre zložitejšie operácie, ktoré vyžadujú uchovávanie stavu a riadenie postupnosti udalostí.
##### Zvoľte si a vyjadrite v binárnom kóde IPv4 adresu s prefixom 24
```
192.168.1.0/24
11000000.10101000.00000001.00000000/24
```
##### Porovnajte IPv4 siete a IPv4 hosta
- IP adresa siete nemá žiadné bity 1 v hostovskej časti
	- IP hosťa má bity 1 v hostovskej časti, preto vieme že je to hostovská IP adresa