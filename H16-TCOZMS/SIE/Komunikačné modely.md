	
a)
1. Definujte vrstvový komunikačný model OSI a model TCP/IP
2. Popíšte spôsob komunikácie medzi jednotlivými vrstvami modelu, použite obrázok 1 obrazovej prílohy č.6
	komunikujú pomocou protokolov (súbory pravidiel)
	fyzická vrstva - signály, vlastnosti, typy, kódovanie technické parametre
	datalinkóvá vrstva - sieťová karta - hardware, software, logická-fizická (mac, a llc)
1. Popíšte proces encapsulácie a deencapsulácie
2. Vysvetlite pojem PDU, použite obrázok 2 obrazovej prílohy č. 6
3. Porovnajte hlavičky PDU Frame a Packet
b)
1. Zdôvodnite potrebu použitia verejných a privátnych IP adries v IPv4
	10.0.0.0/8, 172.168.0.0./16, 192.168.0.0/24 127.0.0.0 lopback
1. Uveďte názvy aspoň dvoch organizácií zodpovedných za otvorené štandardy v sieťach
2. Vysvetlite využitie protokolu NAT
	preklad súkromných adries na verejné
	access listy, statické, dynamické, pat
c)
1. Uveďte výhody a nevýhody jednotlivých zdrojov, metód získavania nových zamestnancov a popíšte základné náležitosti pracovnej zmluvy
2. Vysvetlite pojem algoritmus z hľadiska programovania a vymenujte jeho základné vlastnosti

---
1. **Definícia vrstvových komunikačných modelov OSI a TCP/IP:**
   - **OSI model (Open Systems Interconnection model)** je teoretický model pre sieťové komunikácie, ktorý rozdeľuje komunikačný proces do siedmich vrstiev: Fyzická, Dátová spojová, Sieťová, Transportná, Relačná, Prezentačná a Aplikačná.
   - **TCP/IP model** je praktickejší a používaný v reálnych sieťach. Má štyri vrstvy: Sieťové rozhranie, Internetová, Transportná a Aplikačná. Tento model je základom internetu.

2. **Spôsob komunikácie medzi jednotlivými vrstvami modelu:**
   - V oboch modeloch, OSI a TCP/IP, komunikácia medzi vrstvami prebieha vertikálne. Každá vrstva poskytuje služby vrstve nad sebou a spolieha sa na služby vrstvy pod sebou. Dáta sa pri prechode smerom nadol (od aplikačnej k fyzickej vrstve) balia (encapsulujú) a pri prechode smerom nahor (od fyzickej k aplikačnej vrstve) rozbaľujú (deencapsulujú).

3. **Proces encapsulácie a deencapsulácie:**
   - **Encapsulácia** je proces, pri ktorom každá vrstva pridáva k dátam svoju hlavičku (a niekedy aj pätičku), čím vytvára novú dátovú jednotku pre prenos na nižšiu vrstvu. 
   - **Deencapsulácia** je opačný proces, pri ktorom každá vrstva odstraňuje hlavičku (a pätičku) pridanú predchádzajúcou vrstvou, aby mohla spracovať alebo preposlať dáta vyššej vrstve.

4. **Pojem PDU (Protocol Data Unit):**
   - PDU je jednotka dát, ktorá sa prenáša medzi dvoma vrstvami komunikačného modelu. Každá vrstva má svoj typ PDU: napríklad, v OSI modeli, Frame na dátové spojovej vrstve, Packet na sieťovej vrstve a Segment na transportnej vrstve.

5. **Porovnanie hlavičiek PDU Frame a Packet:**
   - **Frame** (Rámec) je PDU dátové spojovej vrstvy a obsahuje hlavičku s adresami zariadení na lokálnej sieti (MAC adresy), typ dát a kontrolu chýb.
   - **Packet** (Paket) je PDU sieťovej vrstvy a obsahuje hlavičku s logickými adresami (IP adresy) pre doručenie paketu z jedného hostiteľa na druhého cez sieť.

6. **Potreba použitia verejných a privátnych IP adries v IPv4 a úloha NAT:**
   - Verejné IP adresy sú unikátne v celom internete, zatiaľ čo privátne IP adresy sú určené pre použitie v lokálnych sieťach a nie sú unikátne. NAT (Network Address Translation) umožňuje viacerým zariadeniam v lokálnej sieti zdieľať jednu verejnú IP adresu pre prístup na internet, čím zvyšuje bezpečnosť a šetrí verejné IP adresy.

7. **Organizácie zodpovedné za otvorené štandardy v sieťach:**
   - **IETF (Internet Engineering Task Force)** a **IEEE (Institute of Electrical and Electronics Engineers)** sú dve hlavné organizácie, ktoré vyvíjajú a udržiavajú otvorené štandardy pre sieťové technológie.

8. **Porovnanie half-duplex a full-duplex z pohľadu použitého média:**
   - **Half-duplex** režim umožňuje komunikáciu v oboch smeroch, ale nie súčasne. Príkladom môže byť walkie-talkie.
   - **Full-duplex** režim umožňuje súčasnú komunikáciu v oboch smeroch, ako je to napríklad pri telefónnom hovore.

9. **Využitie protokolov pre IPTV a HTTP:**
   - **IPTV (Internet Protocol Television)** využíva sieťové protokoly, najmä IP multicast, pre distribúciu televízneho obsahu cez IP siete, čo umožňuje poskytovanie televíznych služieb cez internetovú infraštruktúru.
   - **HTTP (Hypertext Transfer Protocol)** je základný protokol používaný na prenos dát na webe, najmä webových stránok vo formáte HTML a súvisiacich súborov.