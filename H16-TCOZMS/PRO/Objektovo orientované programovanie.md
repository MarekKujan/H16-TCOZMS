a)
1. Porovnajte objektovo orientované programovanie s procedurálnym programovaním
2. Charakterizujte základné pojmy OOP – trieda, členy tried, objekt
3. Vymenujte prístupové modifikátory a vysvetlite ich význam
4. Charakterizujte prístupové metódy
5. Uveďte, ako sa objekty konštruujú a deštruujú
b)
1. Popíšte, aký je rozdiel medzi nestatickými a statickými členmi tried
2. Charakterizujte dedičnosť', vysvetlite, akým spôsobom je volaný konštruktor bázovej triedy a čo znamená predefinovanie metódy
3. Vytvorte program, v ktorom z bázovej triedy odvodíte novú triedu
c)
1. Popíšte proces encapsulácie na PDU
2. Charakterizujte ekonomické a alternatívne ukazovatele celkovej úrovne bohatstva krajiny

---

- Porovnajte objektovo-orientované programovanie a procedurálne programovanie (ChatGPT)
	**Objektovo-orientované programovanie**
	- _Zameranie:_ Zamieňa sa na objekty a ich vzájomné vzťahy.
	- _Objekty:_ Program sa skladá z objektov, ktoré majú vlastnosti a metódy.
	- _Vzťahy:_ Objekty môžu medzi sebou komunikovať a interagovať.
	- _Zapúzdrenie:_ Objekty zapúzdrujú svoje dáta a metódy, čo zaisťuje lepšiu modulárnu štruktúru.
	- _Dedičnosť:_ Objekty môžu dediť vlastnosti a metódy z iných objektov.
	- _Polymorfizmus:_ Objekty môžu mať rôzne formy a môžu byť použité vo viacerých kontextoch.
	**Procedurálne programovanie**
	- _Zameranie:_ Zamieňa sa na postupnosť krokov alebo funkcií.
	- _Funkcie:_ Program sa skladá z funkcií, ktoré vykonávajú určité operácie.
	- _Kroky:_ Program prechádza postupne cez jednotlivé kroky alebo funkcie.
	- _Štruktúra dát:_ Štruktúra dát je zväčša lineárna a manipulácia s dátami je priamočiara.
	- _Štruktúra programu:_ Program sa skladá z funkcií, ktoré môžu byť zložené do rôznych modulov alebo súborov.
	- _Optimalizácia:_ Optimalizácia je zvyčajne dosiahnutá pomocou procedurálneho prístupu k programovaniu.
- Základné pojmy OOP - trieda, členy tried, objekt
	- trieda je šablóna, vzor, ktorá obsahuje všetky premenné (vlastnosti) a metódy
	- trieda obsahuje konštruktor čo vytvára objekt
	- členmi triedy sú všetky jej vlastnosti a metódy, ktoré sa v nej nachádzajú
	- objekt je daná inštancia triedy, má vlastný názov a rezervované miesto v pamäti
- Prístupové modifikátory a ich význam (stačí 3)
	- Modifikátory prístupu v OOP určujú, kto môže pristupovať k členom triedy (premenným, metódam, getterom, setterom)
	- Tieto modifikátory sú: public, private, protected.
	- K public členom môžeme pristupovať priamo a dajú sa dediť.
	- Protected členy -  prístup k ním je utajený ale jeho vlastnosti môžu dediť  podradené triedy
	- Privátne členy sú prístupné len k objektu. Vytvárame metódy na prístup k premenným. (getter, setter)
- Prístupové metódy, čo sú a na čo slúžia, príklady
	- pristupujú k privatným premenným v objekte
	- getter a setter
- Konštrukcia a deštrukcia objektov (medzi C++ a C# je veľký rozdiel)
	- konšturktor ma rovnaké meno ako trieda
	- vieme ho preťažiť, je public
	- deštruktor v cpp sa volá ak je objekt mimo scope programu alebo ak použijeme funkciu delete()
	- deklaruje sa ako ~trieda()
	- kompilátor má predvolený deštruktor ak nespecifikujeme vlastný
	- v C# sa volajú finalizéri
	- slúžia na dokončenie vyčistenia keď objekt pozbiera garbage collector
	- trieda môže mať jeden deštruktor, nedá sa dediť alebo preťažiť
	- nedajú sa volať, spustia sa automaticky
- Statické a nestatické členy triedy
	- statické metódy patria triede samotnej, môžeme ich volať bez vytvorenie objektu
	- statické premenné patria rovnako triede, napr. inkrementácia statickej hodnoty v objekte zvyšuje počet v tej jednej statickej premennej
	- nestatické metódy sú priradené k objektu, volamé ich cez objekt
	- stále majú prístup k statickým členom
- Dedičnosť – volanie konštruktorov základnej triedy, predefinovanie... a pripraviť kratučký program, trieda, 2 premenné, prístupové metódy, iná trieda
	- 
- ekon. téma: Charakterizujte ekonomické a alternatívne ukazovatele celkovej úrovne bohatstva krajiny
	- vysvetlené v súbore EKN - Témy