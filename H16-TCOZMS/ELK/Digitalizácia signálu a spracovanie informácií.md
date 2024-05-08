---
share: "true"
---
## A
- Nakreslite a popíšte rozdiely medzi analógovým a, číslicovým a digitálnym signálom
- Objasnite parametre reálneho digitálneho signálu, ako aj spôsob a význam digitalizácie signálov
- `popíšte PDU L2`
- `popíšte spôsoby komunikácie half duplex a full duplex`
- `Ekonomická otázka`
## B
- Popíšte význam a princíp činnosti posuvných registrov a časovačov TON a TOFF
- `komunikácia na spoločnom médiu`
- `spôsoby komunikácie medzi switchmi na L2`
## C
- Nakreslite a popíšte jednoduchú schému logického obvodu
- `MAC tabuľka`

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
##### popíšte PDU L2
![[2- tema#^161e64]]
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









