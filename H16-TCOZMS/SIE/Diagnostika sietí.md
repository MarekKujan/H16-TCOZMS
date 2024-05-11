a)
1. Vysvetlite zásady diagnostiky problémov v počítačových sieťach na RM OSI a TCP/IP
  - protokoly a programy fungujú len v rámci vlastnej vrstvy, predávajú si medzi sebou dáta pomocou enkapsulácie, deenkapsulácie
  - porucha sa najčastejšie vyskytuje len na jednej vrstve
  - ak je porucha na nižšej vrstve, nebude fungovať nič na vyššej vrstve
  - prístup k diagnostike problémov, môžeme začať hore alebo dole na relačnom modeli
2. Vymenujte základné softvérové nástroje pre diagnostiku počítačovej siete
  - ping - odošle správu protokolu ICMP a čaká na odpoveď
  - tracert - ako ping ale odpoveď očakávame z každého hopu až k deštinačnej adrese
  - wireshark - program na zachytávanie packetov na našom zariadení
  - debugovacie správy na cisco zariadeniach - široká škála nastavení, výpis debugovacích správ do konzoly, po dokončení diagnostiky treba vypnúť lebo zahlcuje výkon sieťových zariadení 
3. Načrtnite spôsoby nastavenia požadovaných parametrov na routeri (meno, IP adresy, konzola, ...)
  1. vstup do privilegovaného módu IOS, ďalej na konfiguračný mód
  2. IP adresy sa konfigurujú na úrovni rozhrania alebo sub-interfaces
  3. veci ako meno, heslo sú v globálnom konfiguračnom móde
  4. konzola sa zabezpečuje cez line con 0, podobne aj vzdialené manažovanie cez SSH/telnet na line vty
4. Popíšte postup pre overenie konektivity ľubovoľného koncového zariadenia v počítačovej sieti
   - najľahší spôsob je cez ping
   - tu si vieme overiť fungovanie vrstiev 1 až 3 (protokol ICMP je na 3. vrstve ako IP) čo je všetko potrebné pre overenie konektivity
5. Uveďte postup pre zobrazenie nastavených parametrov na sieťovom zariadení
   - ```show running-config``` - výpis každého príkazu, ktorý sme nakonfigurovali na zariadení
   - ostatné príkazy sú specificky určené vždy na protokol alebo službu ktorá beží na zariadení
   - ako príklad: ```show ip interfaces brief, show int trunk, show vlan brief```
b)
1. Vysvetlite dôvody a spôsoby kryptovania hesiel na sieťových zariadeniach
   - kryptovanie hesiel na zariadeniach Cisco
       - v global config móde príkaz: ```service password-encryption```
       - pri zabezpečovaní prístupu cez vty,con,lokálny účet ```enable secret HESLO```
   - ľudia čo sa dostanú do globálneho módu si nevedia skontrolovať heslo pomocou príkazu ```show running-config``` lebo tento príkaz vypiše len jeho enkryptovanú podobu
2. Popíšte možnosti diaľkového prístupu k sieťovým zariadeniam
   - telnet - nezabezpečený diaľkový prístup, príkazy sa posielajú v plaintext
   - SSH - kryptovaný protokol na diaľkový prístup, prihlásenie cez meno/heslo alebo privátny kľúč, kľúče sa generujú cez RSA
3. Vysvetlite význam protokolu ARP
   - Adress Resolution Protocol
   - slúži na objavenie MAC adries na lokálnej sieti a priradenie k príslušnej adrese na L3
   - packety IP musia byť enkapsulované do Framu, ak chýba deštinačná MAC adresa použijeme protokol ARP
   - vysiela sa broadcast ARP request, odpoveď dostáva od zariadenia, ktorého MAC adresu hľadáme vo forme ARP Reply
   - bezpečnosť na sieti: existujú tzv. gratuitous ARP replies, ktoré môže počitač poslať bez ARP Request packetu, nebezpečie spočíva v prepisovaní MAC adries DG, firewall -> Man in the Middle útok (framy sú presmerované na zariadenie hackera)
c)
1. Popíšte diagnostiku a odstraňovanie porúch v navrhnutej počítačovej sieti, použite obrazovú prílohu č. 12
   - diagnostika spočíva v zbieraní symptómov
   - potom ak máme dostatok skúseností môžeme dať odhad o charaktere poruchy
   - podľa typu poruchy vieme využíť viacero troubleshootovacích prístupov
   - najvyužívanejšie sú zhora nadol alebo zdola nahor
   - postupujeme podľa modelu OSI a verifikujeme funkcionalitu
   - vrstvy si môžeme taktiež rozdeliť v štýle Divide and Conquer, kde overíme funkcionalitu jednej vrstvy v strede modelu a odtiaľ sa vydáme logickejším smerom
2. Charakterizujte polia, predveďte deklaráciu a vytvorenie poľa aj z hľadiska pamäte
   - pole je vlastne veľa premenných uložených vedľa seba v pamäti
   - najčastejšie statické polia - nemenná velkosť
   - deklaracia -  hovorime kompilatoru ze budeme vyuzivat premennu v kode
   - vytvorenie - incilizacia je samotne uvedenie premennej do pouzivania, priradime jej adresu v pamati
