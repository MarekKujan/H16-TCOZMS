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
 - Analógovy signál - je spojitý, môže nadobudnút ľubovolnú hodnotu, informáciu nesie amplitúda signálu
 - Digitálny signál - diskrétny, nespojitý signál, informácie tu reprezentuje binárne kódovanie signál je buď HIGH alebo LOW (HIGH - 1, LOW - 0)
##### Objasnite parametre reálneho digitálneho signálu, ako aj spôsob a význam digitalizácie signálov
![[realny_signal.png]]
Digitalizácia signálu je proces prevodu analógového signálu na digitálny formát. Tento proces sa skladá z dvoch hlavných krokov:
1. Vzorkovanie (sampling): Analógový signál je zachytený v určitých časových intervaloch a získané vzorky sú reprezentáciou hodnôt signálu v týchto okamihoch.
2. Kvantizácia (quantization): Hodnoty vzoriek signálu sú zaokrúhlené alebo zaokrúhlené na najbližšiu hodnotu, ktorú je možné reprezentovať v digitálnom formáte. Tým sa dosiahne diskretizácia signálu.
Digitalizácia signálu je dôležitá, pretože umožňuje ukladanie, prenos a spracovanie signálov pomocou digitálnych zariadení. Digitálne signály sú odolnejšie voči šumu a môžu byť ľahko spracované pomocou rôznych algoritmov a techník.

1. popíšte PDU na L2 ^161e64
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
2. popíšte spôsoby komunikácie half duplex a full duplex
	- Half-Duplex
		- médium je schopné len jednosmernej komunikácie
		- starý ethernet štandard pomocou Hubov, Coaxial
		- Ethernet bol elektricky vždy schopný full-duplex, limitáciou nie je kábel ale sieť okolo neho (1. pár - TX, 2. pár - RX, 3. pár - napájanie, 4. pár - rezerva)
			- Ethernet huby boli lacnejšie zariadenia t. j. CSMA-CD, zariadenie museli počúvať či niekto posiela keď oni vysielali aby detegovali kolíziu
		- WLAN siete
		- Jedno vlákno optiky je half-duplex, moderná optika už vie full-duplex
	- Full-Duplex
		- médium je obojsmerné, zariadenie môže vysielať aj prijímať informácie naraz
3. vysvetlite spôsob komunikácie na spoločnom médiu
	- dva métody prístupu CSMA-CD, CSMA-CA
	- CSMA-CD - collision detection - ethernet half-duplex
	- CSMA-CA - collision avoidance - bezdrôtové siete
##### `popíšte spôsoby komunikácie half duplex a full duplex`
#####  Popíšte význam a princíp činnosti posuvných registrov a časovačov TON a TOFF
Posuvné registre sú dôležitou súčasťou digitálnych obvodov a slúžia na uchovávanie a posúvanie dát. Majú široké využitie v rôznych aplikáciách, ako napríklad v sériových komunikačných protokoloch, v riadiacich systémoch alebo v digitálnych hodinách.
Princíp činnosti posuvných registrov spočíva v tom, že dáta sú postupne posúvané z jednej bunky do druhej. Existujú rôzne typy posuvných registrov, ako napríklad posuvné registry s posúvaním vpravo (SISO), posúvaním vľavo (SIPO), posúvaním v oboch smeroch (PIPO) alebo posúvaním v kruhu (PISO).
Posuvné registre sa často používajú v spojení s časovačmi TON (On Delay Timer) a TOFF (Off Delay Timer). Tieto časovače slúžia na oneskorenie alebo oneskorené vypnutie signálu.
Časovač TON je časovač s oneskoreným spustením. Po aktivácii vstupného signálu sa časovač spustí a po uplynutí nastaveného času generuje výstupný signál. Ak je vstupný signál vypnutý pred uplynutím času, časovač sa zastaví a výstupný signál sa nevygeneruje.
Časovač TOFF je časovač s oneskoreným vypnutím. Po aktivácii vstupného signálu sa časovač spustí a po uplynutí nastaveného času vypne výstupný signál. Ak je vstupný signál vypnutý pred uplynutím času, časovač sa zastaví a výstupný signál sa nevypne.
##### `komunikácia na spoločnom médiu`
##### `spôsoby komunikácie medzi switchmi na L2`
##### Nakreslite a popíšte jednoduchú schému logického obvodu
![[log_obvody.png]]
##### `MAC tabuľka`
- tabuľka MAC adries, priradená k portom na switchi
- switch robí prepínacie rozhodnutia na základe tejto tabuľky
- napr. pri cut-through switching, switch si načíta rámec po deštinačnú MAC adresu a začne ho prepínať na port
- naplnenie MAC tabuľky sa deje keď príde rámec na port a zapíše sa jeho source adresa
- ak swtich nemá v MAC tabuľke deštinačnú adresu rámca tak rámec daľej posiela na každý port okrem toho, na ktorom ho dostal









