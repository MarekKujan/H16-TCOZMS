	
- definujte vrstvový komunikačný model OSI a model TCP/IP
- popíšte spôsob komunikácie medzi jednotlivými vrstvami modelu
- popíšte proces encapsulácie a deencapsulácie
- vysvetlite pojem PDU
- porovnajte hlavičky PDU Frame a Packet
- zdôvodnite potrebu použitia verejných a privátnych IP adries v IPv4 a úlohu
NAT
- uveďte aspoň dve organizácie zodpovedné za otvorené štandardy v sieťach
- porovnajte halfduplex a fullduplexz pohľadu použitého média
- vysvetlite využitie protokolov pre IPTV a HTTP

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