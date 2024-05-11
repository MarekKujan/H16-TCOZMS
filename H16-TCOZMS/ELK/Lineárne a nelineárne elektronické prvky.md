a)
1. Porovnajte rozdiel medzi lineárnymi a nelineárnymi elektronickými prvkami
2. Vysvetlite princíp merania odporu priamou a nepriamou metódou
3. Vysvetlite rozdiel medzi ideálnymi a reálnymi elektronickými prvkami
4. Porovnajte správanie sa prvkov R, L a C v obvodoch jednosmerného a striedavého prúdu
5. Určte hodnotu predradného odporu LED diódy s prahovým napätím 2V, ktorou má pretekať prúd 20 mA, ak je napájacie napätie 12 V
b)
1. Popíšte proces nábehu pri zapnutí zariadenia switch - LED diódy
2. Definujte úlohy fyzickej vrstvy modelu OSI
3. Popíšte TP káble
c)
1. Načrtnite štruktúru optických káblov
2. Zaraďte PC do majetku podniku a popíšte jeho obstaranie, ocenenie ako dlhodobého majetku

---
##### Porovnajte rozdiel medzi lineárnymi a nelineárnymi elektronickými prvkami
 - Rozdiel medzi nimi spočíva v ich VACH charakteristike a spôsobe, akým menia prúd alebo napätie.
- **Lineárne elektronické** prvky majú lineárnu charakteristiku, čo znamená, že menia prúd alebo napätie v proporčnom vzťahu. To znamená, že ak sa prúd alebo napätie zmení o určitý faktor, zmení sa aj výstupný signál o rovnaký faktor. Príkladmi lineárnych elektronických prvkov sú rezistory, kondenzátory a induktory.
- **Nelineárne elektronické** prvky majú nelineárnu charakteristiku, čo znamená, že menia prúd alebo napätie v nelineárnom vzťahu. To znamená, že zmena vstupného signálu nemusí mať rovnaký vplyv na výstupný signál. Príkladmi nelineárnych elektronických prvkov sú diódy, tranzistory a operačné zosilňovače.
##### Vysvetlite princíp merania odporu priamou a nepriamou metódou
- Metóda merania odporov **Volt-Ampérovou metódou** je postup, pri ktorom sa meria napätie a prúd v obvode a následne sa vypočíta odpor pomocou Ohmovho zákona. Meranie sa vykonáva pomocou voltmetra a ampérmetra. 
- **Priama metóda** Pri priamej metóde sa odpor meria priamo pomocou odporového meradla, ako je multimeter. Multimeter je zariadenie, ktoré môže merať rôzne elektrické vlastnosti, vrátane odporu. Priame meranie zahŕňa pripojenie zariadenia na meraný odpor a priame zobrazenie jeho hodnoty na displeji.
##### Vysvetlite rozdiel medzi ideálnymi a reálnymi elektronickými prvkami
**Ideálne elektronické prvky:**
- Nemajú žiadny vnútorný odpor alebo straty energie
- Ich parametre sú konštantné a nezávislé na teplotnej alebo iných podmienkach.
- Napríklad ideálny rezistor má presne danú hodnotu odporu bez akejkoľvek variácie.
**Reálne elektronické prvky**:
- Majú vnútorný odpor a straty energie.
- Ich parametre môžu byť ovplyvnené teplotou, frekvenciou, napätím a ďalšími faktormi.
- Napríklad reálny rezistor môže mať malý vnútorný odpor a jeho hodnota sa môže mierne meniť v závislosti od teploty a ďalších faktorov.
##### Porovnajte správanie sa prvkov R, L a C v obvodoch jednosmerného a striedavého prúdu
**Jednosmerný prúd:**
- **Rezistor (R):** V obvode s jednosmerným prúdom sa správa rezistoru nezmení. Rezistor jednoducho obmedzuje prúd, ktorý cez neho prechádza, a konvertuje elektrickú energiu na teplo podľa Ohmovho zákona (U = IR).
- **Cievka (L):** Pri jednosmernom prúde sa induktor správa ako otvorený obvod. To znamená, že sa správa ako veľmi veľký odpor pre jednosmerný prúd, takže takmer žiadny prúd nekrúti. Jeho jednosmerný odpor je teoreticky nekonečný.
- **Kondenzátor (C):** Pri jednosmernom prúde sa kondenzátor správa ako krátky obvod. To znamená, že v okamihu zapnutia kondenzátoru sa všetka energia akumulovaná v elektrickom poli na ňom vyčerpá. Jeho jednosmerný odpor je teoreticky nulový.
**Striedavý prúd:**
- **Rezistor (R):** Správanie rezistoru v obvode so striedavým prúdom je rovnaké ako pri jednosmernom prúde. Rezistor jednoducho obmedzuje prúd podľa Ohmového zákona a mení elektrickú energiu na teplo.
- **Cievka (L):** Pri striedavom prúde sa induktor správa ako zložitý prvok, ktorý vytvára magnetické pole, ktoré sa mení v čase. V dôsledku toho vzniká indukované napätie, ktoré spôsobuje v obvode proti prúdu. Tento efekt spôsobuje zdĺhavý nárast prúdu cez induktor.
- **Kondenzátor (C):** Pri striedavom prúde sa kondenzátor správa ako zložitý prvok, ktorý uchováva náboj a vytvára elektrické pole. Pri meniacom sa napätí na kondenzátore sa náboj pohybuje dovnútra a von z kondenzátora v závislosti od polarity napätia, čo vedie k prúdu.
![[Pasted image 20240511114517.png]]
##### Určte hodnotu predradného odporu LED diódy s prahovým napätím 2V, ktorou má pretekať prúd 20mA ak je napájacie napätie 12V
- Hodnota predradného odporu LED diódy sa dá vypočítať pomocou Ohmovho zákona. Ohmov zákon hovorí, že napätie na odporovom prvku je rovné súčinu prúdu a odporu.
- V tomto prípade máme napájacie napätie (V) = 12V, prúd (I) = 20mA (čo je 0.02A) a prahové napätie LED diódy (V_LED) = 2V.
Predradný odpor (R) sa dá vypočítať ako:
R = (V - V_LED) / I
R = (12V - 2V) / 0.02A
R = 10V / 0.02A
R = 500Ω
##### Popíšte proces nábehu pri zapnutí zariadenia switch - LED diódy
- **Step 1**: First, the switch loads a power-on self-test (POST) program stored in ROM. POST checks the CPU subsystem. It tests the CPU, DRAM, and the portion of the flash device that makes up the flash file system.  
- **Step 2**: Next, the switch loads the boot loader software. The boot loader is a small program stored in ROM that is run immediately after POST successfully completes.  
- **Step 3**: The boot loader performs low-level CPU initialization. It initializes the CPU registers, which control where physical memory is mapped, the quantity of memory, and its speed.  
- **Step 4**: The boot loader initializes the flash file system on the system board.  
- **Step 5**: Finally, the boot loader locates and loads a default IOS operating system software image into memory and gives control of the switch over to the IOS.
![[Pasted image 20240511120429.png]]
- **System LED** Shows whether the system is receiving power and is functioning properly.
- **Redundant Power System (RPS) LED**
- **Port Status LED** Indicates that the port status mode is selected when the LED is green.
- **Port Duplex LED** Indicates that the port duplex mode is selected when the LED is green.
- **Port Speed LED** Indicates that the port speed mode is selected.
- **Power over Ethernet (PoE) Mode LED**
##### Definujte úlohy fyzickej vrstvy modelu OSI
**Fyzická vrstva modelu OSI**  Je zodpovedná za fyzickú prenosovú a prijímaciu časť dát medzi zariadeniami a riadi prístup k fyzickému médium, ako sú koaxiálne káble, optické vlákna alebo bezdrôtové prenosové médium. Tu sú hlavné úlohy fyzickej vrstvy:
- **Prepojenie fyzického média:** Fyzická vrstva umožňuje prenos dát cez rôzne typy fyzických médií, ako sú káble, vlákna alebo bezdrôtové prenosové médiá. Zabezpečuje, že dáta sú vhodne zakódované pre dané médium a prenášajú sa cez správne.
- **Synchronizácia dátových rámcov:** Fyzická vrstva zabezpečuje, že dáta sú prenášané v správnom čase a že odosielateľ a prijímateľ sú synchronizovaní. To zahŕňa koordináciu bitov na fyzickom médiu tak, aby boli dáta presne prenesené a následne interpretované správne.
- **Fyzická topológia siete:** Fyzická vrstva definuje fyzickú topológiu siete, teda spôsob, ako sú zariadenia pripojené a ako sú spojené s prenosovými médiami. Môže ísť o hviezdicovú, kruhovú, zbernicovú alebo inú topológiu, ktorá ovplyvňuje spôsob, ako sa dáta fyzicky prenášajú.
- **Kódovanie a modulácia signálu:** Fyzická vrstva zahŕňa procesy kódovania a modulácie signálu, ktoré umožňujú prevádzať digitálne dáta na analógový signál pre prenos cez fyzické médium a následné dekódovanie a demoduláciu na prijímateľskej strane.
#####  Popíšte TP káble
- káble Twisted Pair, 4 páry vodičov ktoré sú krútené aby minimalizovali crosstalk
- crosstalk je jav kde sa indukuje napätie na susedné vodiče, krútenie tieto elektromagnetické javy vynuluje
- UTP, FTP, STP káble - rôzne stupne ochrany pred rušením z vonkajších zdrojov ako je vedenie napájnia
- existujú rôzne kategórie, rozlišné prenosové rýchlosti
- káble TP končia koncovkou RJ45, 2 štandary TIA/EIA 568A-B
- káble možno ďalej rozdeliť na: straight-through, crossover

#####  Načrtnite štruktúru optických káblov
![[Pasted image 20240511123153.png]]
##### [[EKN#Zaraďte PC do majetku podniku a popíšte jeho obstaranie, ocenenie ako dlhodobého majetku]]
