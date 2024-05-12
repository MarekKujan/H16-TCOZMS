a)
1. Popíšte typy sieťových adaptérov (sieťových kariet)
   - metalické, používaju normálne elektrinu na prevedenie signálu
   - optické, vysielaju svetlo a prijímaju pomocou optického transciver (transmitter a receiver)
   - bezdrôtové, signál sa šíri EM vlnami
3. Definujte priradenie sieťového adaptéra ku konkrétnej vrstve RM OSI
   - rozhranie a a hadrvér sieťovej karty patrí na Vrstvu L1
   - cieľom sieťovej karty je enkódovať údaje tak aby boli prenositeľné na médiu
   - ovládač a údaje ktoré putujú v signály patria na vrstvu L2
5. Vysvetlite štruktúru MAC adresy
   - 6 párov hexadecimálnych znakov (48)
   - prvé 3 páry - časť registrovaná výrobcovi
   - zvyšné 3 - náhodne generované, unikátne pre sieťovú kartu
7. Kategorizujte rozhranie sieťových adaptérov pre metalické médiá
   - rozhranie robí fyzický kontakt s médiom, používa elektrické napätie na odosielanie signálu
   - RJ45, Coaxial, serial
9. Zdôvodnite potrebu ARP protokolu
   -pomáha na objavenie MAC adries ostatných hostov na viacprístupovej sieti ako je ethernet (multi-access network)
b)
1. Definujte normu 568B a 568A
   - je to norma, ktorá udáva poradie terminovania káblov na konektori RJ-45
   - existuje verzia A aj B, kombinácia dvoch verzií nám vyrobí ethernet kábel typu crossover
   - rovnaká verzia na oboch koncoch -> straight-through
2. Popíšte rámec Ethernet
  - Frame je PDU na vrstve L2
	- enkapsuluje PDU z L3 (packet)
	- pridáva Header a Footer
	- Header obsahuje minimálne
		- Preambula 10101010 * 7 bajtov
		- Start Frame Delimiter 101010**11**
		- MAC adresy: source a destination, pre WLAN možú byť ešte zvyšné 2 MAC adresy
		- protokol na vyššej vrstve
	- samotný packet
	- Footer
		- FCS (Frame Check Sequence)
		- systém na overenie či vo frame nedošlo k porušeniu údajov
3. Vysvetlite, ako switch napĺňa tabuľku MAC adries, použite obrazovú prílohu č. 10
  - napĺňa ju pomocou source MAC adresy v rámci na prichádzajúcom porte
  - ak switch nemá v MAC tabuľke adresu deštinačného zariadenia tak swtich prepošle frame na každý port okrem toho na ktorý dorazil
c)
1. Zaraďte počítač do majetku podniku a popíšte formy jeho opotrebenia a odpisovania v podniku
2. Vymenujte relačné a logické operátory a vysvetlite ich význam a spôsob použitia
