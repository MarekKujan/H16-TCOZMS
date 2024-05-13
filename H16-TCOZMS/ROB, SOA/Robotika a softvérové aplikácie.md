a)
1. Uveďte, čo je to Arduino, popíšte jeho základné časti
2. Popíšte využitie servomotora v praxi
3. Porovnajte pojmy robot a robotický manipulátor
4. Vysvetlite pojem kinematická štruktúra, použite prílohu č. 25
5. Vymenujte a popíšte typy podvozkov mobilných robotov
b)
1. Odvoďte polomer otáčania diferenciálneho podvozku
2. Porovnajte optický inkrementálny a absolútny snímač polohy
3. Vytvorte program, v ktorom bude blikať LED s periódou 0.5s
c)
1. Vysvetlite znaky, funkcie a právne formy podniku na Slovensku
2. Charakterizujte najpoužívanejšie komponenty v aplikáciách s grafickým rozhraním


---

## Arduino, jeho základné časti
- Arduino je mikroovládač
- Skladá sa z: pinov (veľa rôznych funkcií), samotný mikroovládač, USB konektor, pripojenie na zdroj, tlačítko RESET, ICSP (debug a nahrávanie programov), podporné obvody
![[labelled_arduino_parts.png|labelled_arduino_parts.png]]
## Popíšte využitie servomotora v praxi
- Robotická ruka 
- Servomotor vie držať presné uhly, ktoré mu zadáme cez PWM signál
- Preto je ideálny na ovládanie robotickej ruky

## Porovnajte pojmy robot a robotický manipulátor

#### Robot
- všeobecný pojem, ktorý pomenúva stroje alebo zaridenia, ktoré sú schopné vykonávať určité úlohy alebo činnosti s menšou alebo žiadnou ľudskou interakciou

## Vysvetlite pojem kinematická štruktúra
- odvíja sa od konštrukcie konkrétneho druhu
- daná kinematickou štruktúrou, t. j. typ a postupnosť usporiadania kinematických dvojíc
v kinematickom reťazci
- pohybové vlastnosti dané počtom rotačných osí (R) a počtom priamych osí (T)
![[Pasted image 20240513133935.png]]
![[Pasted image 20240513133951.png]]
![[Pasted image 20240513134520.png]]
## Vymenujte a popíšte typy podvozkov mobilných robotov


## Odvodte polomer otáčania deferenciálneho podvozku

 R = (L / 2) * ((v_l + v_r) / (v_r - v_l)) kde:
    - (R) je polomer otáčania,
    - (L) je rozostup medzi kolesami (vzdialenosť medzi ľavým a pravým kolesom),
    - (v_l) je rýchlosť ľavého kolesa,
    - (v_r) je rýchlosť pravého kolesa.
Tento vzorec vychádza z predpokladu, že rýchlosť otáčania ľavého a pravého kolesa je rôzna. Ak by boli rýchlosti rovnaké, vozidlo by sa pohybovalo priamo a polomer otáčania by bol teoreticky nekonečný. Zjednodušenie vzorca:
    
1. **Rozdiel rýchlostí** ((v_r - v_l)) určuje, ako rýchlo sa vozidlo otáča. Ak je tento rozdiel veľký, vozidlo sa otáča rýchlejšie a na menšom polomere. Ak je rozdiel malý, otáča sa pomalšie a na väčšom polomere.
    
2. **Súčet rýchlostí** ((v_l + v_r)) predstavuje celkovú "otáčaciu silu" vozidla. Tento súčet sa delí rozdielom rýchlostí, aby sa získal pomer, ktorý určuje, ako efektívne vozidlo využíva svoju otáčaciu silu na zmenu smeru.
    
3. Nakoniec, celý tento pomer sa násobí polovicou rozostupu kolies ((\frac{L}{2})), čo zohľadňuje fyzickú štruktúru vozidla a jeho schopnosť otáčať sa okolo stredového bodu medzi kolesami.
    
V podstate, tento vzorec hovorí, že polomer otáčania je priamo ovplyvnený tým, ako rôzne sa otáčajú kolesá (rozdiel v ich rýchlostiach) a ako je vozidlo široké (rozostup kolies). Vozidlo sa otáča efektívnejšie (na menšom polomere) s väčším rozdielom v rýchlostiach kolies a menším rozostupom medzi nimi.
## Porovnajte optický inkrementálny a absolútny snímač polohy
- inkrementalny snimac vie snimat pohyb v nejakom smere
- ako priklad myska, opticky snimac porovnava ktorym smerom sa posuva myska a posiela signal, mysku mozete polozit hocikde, snima to len smer pohybu a jej rychlost
- ![[Pasted image 20240503103910.png|Pasted image 20240503103910.png]]
- absolutny snimac polohy snima absolutnu polohu nejakej suciastky
- vyuzivane castejsie v robotike a tak
- ako priklad GPS, viete vasu presnu polohu nie len smer ktorym sa pohybujete
## Vytvorte porgram, v ktorom bude blikať LED 0,5s

```c++\
// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(13, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(13, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(500);                       // wait for a second
  digitalWrite(13, LOW);    // turn the LED off by making the voltage LOW
  delay(500);                       // wait for a second
}
```
## Charakterizujte najpoužívanejšie komponenty v aplikáciach s grafickým rozhraním
Button, TextBox, ComboBox, Scrollbar, Lista nastrojov, Grafika, Context Menu, 

