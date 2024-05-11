a)
1. Nakreslite a popíšte rozdiely medzi analógovým, číslicovým a digitálnym signálom
2. Objasnite význam digitalizácie informácií
3. Popíšte časové priebehy na vstupoch a výstupoch časovačov TON a TOF
4. Popíšte základné kroky potrebné na digitalizáciu analógového signálu
5. Vysvetlite, aké finančné zdroje môže využívať výrobca PC a zaraďte PC do majetku podniku
b)
1. Popíšte PDU na L2
2. Popíšte spôsoby komunikácie half duplex a full duplex
3. Vysvetlite spôsob komunikácie na spoločnom médiu
c)
1. Popíšte MAC tabuľku
2. Popíšte manažovanie switchu na L2

---
##### Nakreslite a popíšte rozdiely medzi analógovým a, číslicovým a digitálnym signálom
![[typy_signalov.png]]
 - **Analógovy signál** - je spojitý, môže nadobudnút ľubovolnú hodnotu, informáciu nesie amplitúda signálu
 - **Digitálny signál** - diskrétny, nespojitý signál, informácie tu reprezentuje binárne kódovanie signál je buď HIGH alebo LOW (HIGH - 1, LOW - 0)
 - **Číslicový signál** - je diskrétny signál, ktorý nadobúda konkrétne a oddelené hodnoty. Nie v každom čase nameriame informáciu
##### Objasnite parametre reálneho digitálneho signálu, ako aj spôsob a význam digitalizácie signálov
![[realny_signal.png]]
Digitalizácia signálu je proces prevodu analógového signálu na digitálny formát. 
Digitalizácia signálu je dôležitá, pretože umožňuje ukladanie, prenos a spracovanie signálov pomocou digitálnych zariadení. Digitálne signály sú odolnejšie voči šumu a môžu byť ľahko spracované pomocou rôznych algoritmov a techník.

##### Popíšte časové priebehy na vstupoch a výstupoch časovačov TON a TOF
![[Pasted image 20240511102323.png]]
##### Popíšte základné kroky potrebné na digitalizáciu analógového signálu
1. **Vzorkovanie (sampling):** Analógový signál je zachytený v určitých časových intervaloch a získané vzorky sú reprezentáciou hodnôt signálu v týchto okamihoch.
2. **Kvantizácia (quantization):** Hodnoty vzoriek signálu sú zaokrúhlené na hodnotu, ktorú je možné reprezentovať v digitálnom formáte. Tým sa dosiahne diskretizácia signálu.
3. **Kódovanie (Encoding):** Každá hodnota signálu je reprezentovaná sériou bitov, ktoré ju identifikujú a umožňujú jej uloženie a spracovanie v digitálnej podobe.
##### [[EKN#Vysvetlite, aké finančné zdroje môže využívať výrobca alebo predajca PC a zaraďte PC do majetku podniku]]

##### Popíšte PDU na L2 
![[Pasted image 20240511105901.png]]
- Frame je PDU na vrstve L2
- enkapsuluje PDU z L3 (packet)
- pridáva Header a Footer
- Header obsahuje minimálne
	- Preambula 1010 * 7 bajtov
	- Start Frame Delimiter 101010**11**
	- MAC adresy: source a destination, pre WLAN možú byť ešte zvyšné 2 MAC adresy
	- protokol na vyššej vrstve
- samotný packet
- Footer
	- FCS (Frame Check Sequence)
	- systém na overenie či vo frame nedošlo k porušeniu údajov
##### Popíšte spôsoby komunikácie half duplex a full duplex
- Half-Duplex
	- médium je schopné len jednosmernej komunikácie
	- starý ethernet štandard pomocou Hubov, Coaxial
	- Ethernet bol elektricky vždy schopný full-duplex, limitáciou nie je kábel ale sieť okolo neho (1. pár - TX, 2. pár - RX, 3. pár - napájanie, 4. pár - rezerva)
	- Ethernet huby boli lacnejšie zariadenia t. j. CSMA-CD, zariadenie museli počúvať či niekto posiela keď oni vysielali aby detegovali kolíziu
	- WLAN siete
	- Jedno vlákno optiky je half-duplex, moderná optika už vie full-duplex
- Full-Duplex
	- médium je obojsmerné, zariadenie môže vysielať aj prijímať informácie naraz
##### Vysvetlite spôsob komunikácie na spoločnom médiu
- dve métody prístupu CSMA-CD, CSMA-CA
- **CSMA-CD** - collision detection - ethernet half-duplex
	- Zariadenie, ktoré chce odoslať dáta, najprv počká na voľné médiá a potom odosiela svoje dáta. Avšak, predtým ako začne odosielať, monitoruje médiá, aby sa uistilo, že nie je žiadny iný prenos v tom istom čase.
- **CSMA-CA** - collision avoidance - bezdrôtové siete
	- **Token Passing:** Tento protokol je používaný v sietiach typu Token Ring, kde je používaný token, ktorý sa pohybuje medzi zariadeniami.
	- Zariadenie môže odosielať dáta len vtedy, keď má fyzicky vlastný token. Po odoslaní dát token prechádza ďalej na ďalšie zariadenie.
#####  Popíšte MAC tabuľku
- tabuľka MAC adries, ktoré sú priradené k portom na switchi
- switch robí prepínacie rozhodnutia na základe tejto tabuľky
- naplnenie MAC tabuľky sa deje keď príde rámec na port a zapíše sa jeho source adresa
- ak swtich nemá v MAC tabuľke deštinačnú adresu rámca tak rámec daľej posiela na každý port okrem toho, na ktorom ho dostal

##### Popíšte manažovanie switchu na L2
- Konfigurácia portov
- Správa VLAN
- Monitorovanie a diagnostika
- Zálohovanie a obnovenie konfigurácie