a)
1. Špecifikujte základné komponenty personálneho počítača strednej triedy
2. Vysvetlite úlohy operačného systému
3. Porovnajte blokovú schému von Neumanovej a Harvardskej architektúry počítača, použite obrazovú prílohu č. 14
4. Definujte formáty základných dosiek s popisom čipovej sady severného a južného mostíka
5. Charakterizujte typy čipov ROM BIOSu
b)
1. Vymenujte a popíšte spôsob použitia niektorých interných pamätí v počítači
2. Vysvetlite vývoj pamäťových modulov RAM v počítači
3. Charakterizujte vývoj a druhy operačných systémov
c)
1. Vysvetlite hlavné úlohy personálneho manažmentu v podniku
2. Charakterizujte objektovo orientované programovanie a vysvetlite základné pojmy: trieda, objekt, členy tried atď.

---
##### Špecifikujte základné komponenty personálneho počítača strednej triedy
1. **Procesor (CPU)**: Srdce počítača, ktoré vykonáva všetky výpočty a operácie. V strednej triede to môže byť viacjadrový procesor s dostatočným výkonom na bežné úlohy ako je práca s dokumentmi, surfovanie po internete alebo hranie hier.
2. **Operačná pamäť (RAM)**: Pamäť používaná na okamžité ukladanie a získavanie údajov pre aktuálne spustené programy a procesy. Počítače strednej triedy môžu mať obvykle 8 GB až 16 GB RAM.
3. **Úložný priestor (pevný disk alebo SSD)**: Slúži na trvalé ukladanie dát, ako sú aplikácie, dokumenty, média atď. Pevné disky s kapacitou 500 GB až 2 TB alebo SSD s podobnými kapacitami sú bežné pre strednú triedu.
4. **Grafická karta (GPU)**: Je zodpovedná za vykresľovanie obrázkov na obrazovke. V počítačoch strednej triedy môže byť integrovaná grafická karta, ktorá zdieľa pamäť s hlavným systémom alebo diskretná grafická karta, ktorá má vlastnú pamäť.
5. **Základná doska (Motherboard)**: Komponent, ktorý spája všetky ostatné komponenty dohromady a umožňuje im komunikovať medzi sebou.
6. **Napájanie (Power Supply Unit - PSU)**: Zdroj energie, ktorý dodáva elektrický prúd do všetkých komponentov počítača.
7. **Chladič a ventilátor(y)**: Chladič udržiava teplotu procesora a iných dôležitých komponentov na bezpečnej úrovni. Ventilátory pomáhajú pri odvádzaní tepla z počítača.
8. **Zvuková karta**: Riadi zvukový výstup a vstup pre reproduktory, slúchadlá, mikrofóny a iné zvukové zariadenia.
9. **Sieťová karta** (Ethernet alebo Wi-Fi):** Umožňuje pripojenie k internetu a lokálnej sieti.
##### Vysvetlite úlohy operačného systému
1. **Správa zdrojov:** Operačný systém riadi prístup k hardvérovým zdrojom, ako sú procesor, pamäť, úložný priestor a periférne zariadenia. Zabezpečuje, aby rôzne programy a procesy mohli zdieľať zdroje efektívne a bezpečne.
2. **Správa súborov:** OS zabezpečuje organizáciu a správu súborov na úložných zariadeniach. To zahŕňa vytváranie, premenu, kopírovanie, premiestňovanie a mazanie súborov a priečinkov. Taktiež zabezpečuje, aby boli súbory chránené pred neoprávneným prístupom a stratením.
3. **Prostredie užívateľa:** Poskytuje užívateľské rozhranie, ktoré umožňuje interakciu s počítačom. To môže zahŕňať grafické používateľské rozhranie (GUI), príkazový riadok alebo iné formy interakcie.
4. **Správa procesov:** Operačný systém riadi spustené programy a procesy, vrátane alokácie procesora, časových plánov, riadenia pamäti a synchronizácie medzi procesmi.
5. **Komunikácia so zariadeniami:** Zabezpečuje komunikáciu s periférnymi zariadeniami, ako sú klávesnice, myši, tlačiarne, monitor, sieťové adaptéry a ďalšie.
6. **Zabezpečenie:** Operačný systém zabezpečuje ochranu pred neoprávneným prístupom, škodlivým softvérom a ďalšími bezpečnostnými hrozbami. To môže zahŕňať prístupovú kontrolu, šifrovanie údajov, firewall a ďalšie bezpečnostné opatrenia.
7. **Správa sietí:** V prípade operačných systémov siete zabezpečuje komunikáciu a správu v rámci lokálnej siete a pripojenie k internetu.
##### Porovnajte blokovú schému von Neumanovej a Harvardskej architektúry počítača, použite obrazovú prílohu č. 14

![[Von-Neuman-Vs-Harvard-Architecture-770544868.png]]
##### Definujte formáty základných dosiek s popisom čipovej sady severného a južného mostíka
![[Pasted image 20240510155029.png]]
- **ATX** – Intel,  veľmi veľké rozšírenie
- **WTX** - Workstation Technology, Intel,  použitie v minulosti hlavne pre servery, v súčasnosti hlavne pre výkonnejšie grafické PC, má odklopné časti a zásuvky, je spätne kompatibilné s ATX
- **BTX**- Balanced Technology, intel, veľmi podobná ATX, predpokladaná náhrada, neúspešná
- **mini-ITX** - malá veľkosť, Intel
- **NLX** - New Low Profile, Intel, pre nízke skrine, zasúva do expandéra

![[Pasted image 20240510192836.png]]
a) North bridge
- rýchla komunikácia s procesorom
- určuje rýchlosť, akou CPU komunikuje so všetkými ostatnými komponentmi v počítači.
- rozhranie voči pamäťovému podsystému
- rozhranie voči zbernici AGP, PCI Express (grafický podsystém)
- komunikácia s južným mostom
b) South bridge
- umožňuje CPU komunikovať so zariadeniami s pomalšou rýchlosťou vrátane pevných diskov, portov Universal Serial Bus (USB) a rozširujúcich slotov.
- rozhranie voči systémovým zariadeniam matičnej dosky (napr. RTC, APM)
- rozhranie voči ďalším komponentom (ISA, COM, LPT, ...)
c) SuperIO
- pripojenie bežných periférii k systému (COM, LPT, FDD, klávesnica, myš).
- pracuje najpomalšie.
- niektoré rozhrania sa pripájajú buď na SuperIO alebo na South Bridge (IDE, USB, CMOS RAM).
##### Charakterizujte typy čipov ROM BIOSu
![[Pasted image 20240510193517.png]]
- P=programming
- E = erasable = vymazateľné ultrafialovým svetlom
- EE = electrically erasable
##### Vymenujte a popíšte spôsob použitia niektorých interných pamätí v počítači
- **operačná pamäť** -je pamäť v ktorej je uložený prebiehajúci program a údaje s ktorými spolupracuje procesor.
- **registre procesora** 
	- je pamäťové miesto, ktoré slúži procesoru na uchovávanie údajov, ktoré práve spracováva
	- ide o pomerne malé množstvo veľmi rýchlej pamäte, ktorá je priamo súčasťou procesorového jadra a prístup k nemu závisí od inštrukčnej sady.	
 - **vyrovnávacia pamäť (buffer)** - je to pracovná pamäť jednotlivých komponentov
- **cache** 
	-  je malá, ale rýchla slúži na prechodné ukladanie dát alebo sekvencií programu
	- spolupracuje priamo s procesorom
	- môže byť externá, alebo interná.

##### Vysvetlite vývoj pamäťových modulov RAM v počítači
![[Pasted image 20240510194141.png]]
##### Charakterizujte vývoj a druhy operačných systémov
- **Skoré operačné systémy:** V skorých dňoch počítačových vedeckých a výskumných laboratórií, v 50. a 60. rokoch 20. storočia, boli operačné systémy základné a veľmi primitívne. Jedným z najznámejších skorých operačných systémov bol UNIX, vyvinutý v laboratóriách Bell Labs v 70. rokoch.
- **Grafické užívateľské rozhrania (GUI):** S nástupom osobných počítačov a návratom spoločnosti Apple na trh s počítačmi s uvedením Macintosh v roku 1984 a neskôr s príchodom Microsoft Windows 3.0 v roku 1990 sa začali objavovať operačné systémy s grafickými užívateľskými rozhraniami
- **Multitasking a multiprocessorové systémy:** S nástupom silnejších hardvérových technológií sa operačné systémy začali vyvíjať s podporou multitaskingu a multiprocessingu. To znamená, že môžu bežať viacero úloh súčasne a využívať viacero procesorov.
**Delenie OS:**
- Podľa počtu používateľov (jedno alebo viac-používateľské)
- Podľa režimu, v ktorom pracuje (grafický alebo textový)
- Podľa počtu úloh, ktoré dokáže vykonávať "súčasne" (jedno alebo viacúlohový (multitasking))
##### [[EKN#Vysvetlite hlavné úlohy personálneho manažmentu v podniku]]

##### Charakterizujte objektovo orientované programovanie a vysvetlite základné pojmy: trieda, objekt, členy tried atď.
- **Objekt:** Objekt je konkrétna inštancia triedy. Znamená to, že objekt je reálna entita, ktorá existuje v pamäti počítača a má svoje vlastné atribúty a môže vykonávať operácie definované v triede, ktorá mu zodpovedá. Objekt je "skutočnou" realizáciou triedy.
- **Členy triedy:** Členy triedy sú vlastnosti a metódy, ktoré sú definované v triede.
- **Atribúty (premenné):** Atribúty triedy sú premenné, ktoré uchovávajú dáta pre každý konkrétny objekt. Môžu reprezentovať stav alebo vlastnosti objektu.
- **Metódy (funkcie/procedúry):** Metódy triedy sú funkcie alebo procedúry, ktoré operujú nad dátami objektu. Môžu meniť stav objektu alebo vykonávať rôzne operácie.
- **Dedičnosť:** Dedičnosť je proces, ktorý umožňuje vytvárať nové triedy (tzv. podtriedy alebo potomkov) na základe existujúcej triedy (tzv. nadtriedy alebo rodiča). Potomky zdedia vlastnosti a metódy nadtriedy a môžu definovať ďalšie špecifické vlastnosti alebo správanie.
