a)
1. Porovnajte konzolové aplikácie s aplikáciami s grafickým rozhraním
2. Uveďte, čo rozumieme pod udalosťami riadenom programovaní
3. Charakterizujte komponenty z hľadiska OOP
4. Popíšte vývojové prostredie v režime tvorby aplikácie s grafickým rozhraním
5. Charakterizujte základné komponenty
b)
1. Vymenujte a popíšte základné vlastnosti komponentov
2. Popíšte obsluhu základných udalosti
3. Vytvorte aplikáciu s grafickým rozhraním, jednoduchú kalkulačku so základnými aritmetickými operáciami a do aplikácie doplňte funkciu na výpočet druhej odmocniny
c)
1. Popíšte PDU na transportnej vrstve
2. Charakterizujte banku a popíšte základné bankové operácie

---

- Porovnanie konzolových aplikácií s aplikáciami s grafickým rozhraním
	1. Konzolové aplikácie:
		- využívajú na vstup a výstup konzolu
		- ide o rozhranie, ktoré ovládam cez klávesnicu
		- väčšinou nejaký príkaz ktorému zadáme argumenty pri volaní
		- aplikácie môžu taktiež vyžadovať údaje počas spustenia
		- najvyspelejšie sú TUI (Text User Interface) programy, pomocou znakov v konzole vytvárajú uživateľské rozhranie
	2. Grafické rozhrania:
		- oveľa prístupnejšie bežnému použivateľovi
		- ovláda sa cez grafické prvky ku ktorým pristupujeme myškou
		- zaberá viac miesta v operačnej pamäti (pre dnešné počitače to nie je problém)
- Udalosťami riadené programovanie – čo to vlastne je (zhrnutie z diplomky od google gemini)
	**Princíp:**
	- Priebeh programu určujú vznikajúce udalosti.
	- Udalosti vznikajú:
	    - Používateľskou akciou (stlačenie tlačidla)
	    - Výstupom senzora
	    - Udalosťou vytvorenou v inej časti programu
	**Použitie:**
	- Prevažne v grafických používateľských rozhraniach (GUI)
	- Kód reaguje na základe používateľského vstupu
	**Implementácia:**
	1. Hlavná slučka (metóda loop()) čaká na prijatie udalosti.
	2. Po prijatí udalosti spustí zaregistrované callback funkcie.
	    - Callback funkcia je funkcia zaregistrovaná v hlavnej slučke ako parameter pre spustenie kódu.
	3. Vstavané systémy:
	    - Hlavná slučka je implementovaná pomocou hardvérových prerušení namiesto aktívnej slučky.
- Komponenty z hľadiska OOP – čo sú komponenty, aspoň 5
	- su to triedy s vlastnymi metodami co asi dedia nejake zakladne vlasnosti a su nadviazane na tu triedu okno kde sa vyskytuju
	- 
- Popis vývojového prostredia
	- softvér, ktorý zľahčuje prácu programátora
	- väčšinou zameraný na jeden konkrétny programovací jazyk
	- obsahuje všetok softvér na prácu s kódom
	- editor text, kompilátor, interpretér, debuger
	- menežovanie komplexných projektov a zdrojových kódov
	- nástroje na vizualizáciu 
- Základné komponenty a ich vlastnosti
	- 
- Obsluha základných udalostí
	- 
- Vytvorte aplikáciu s grafickým rozhraním, jednoduchú kalkulačku s výpočtami
	- 
- Ako by sme riešili nesprávne vstupu, namiesto reťazca napíšeme číslo
	- 
- ekon. téma: Charakterizujte banku a popíšte základné bankové operácie