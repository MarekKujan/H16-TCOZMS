a)
1. Popíšte objekty a metódy používané pri konzolovom výstupe a vstupe
2. Uveďte, ako sú vstupy a výstupy realizované v grafických rozhraniach
3. Definujte pojmy premenná, konštanta a popíšte konverzie medzi reťazcami a číslami
4. Uveďte, na čo slúži operátor priradenia
5. Vymenujte a popíšte aritmetické operátory a ich prioritu
b)
1. Vymenujte a popíšte niektoré matematické funkcie a metódy
2. Popíšte spôsob volania matematických funkcií a metód
3. Vytvorte program na výpočet polomeru kruhu, pri jeho známom obsahu zadanom z klávesnice
c)
1. Zdôvodnite potrebu vysielania broadcast v počítačovej sieti
2. Uveďte aké náklady, výnosy a výsledok hospodárenia vznikajú v podniku (analýza nulového bodu)

---
### Objekty a metódy používané pri konzolovom vstupe a výstupe

**C++:**
```cpp
#include <iostream>
using namespace std;

cout << "text";       // Výstup na konzolu
cin >> string;        // Vstup zo konzoly
```

**C#:**
```csharp
using System;

Console.Write();      // Výstup na konzolu bez nového riadku
Console.WriteLine();  // Výstup na konzolu s novým riadkom
Console.ReadLine();   // Vstup zo konzoly
Console.ReadKey();    // Čaká na stlačenie klávesy
Console.Read();       // Vráti Unicode hodnotu prvého znaku z prúdu vstupu
```

### Ako sú realizované V/V operácie v prípade grafických rozhraní

Vstupné a výstupné operácie sprostredkúvajú volania metód a úpravu parametrov objektu grafického rozhrania, ktorý sa inicializuje pri spustení programu. Tieto operácie môžu zahŕňať zobrazovanie textu, tlačidiel, políčok na zadávanie textu a iných interaktívnych prvkov.

### Popíšte premenné

Premenné reprezentujú úložisko v operačnej pamäti. Každá premenná má typ, ktorý rozhoduje aké hodnoty sa môžú v nej ukladať. Hodnota premennej sa dá zmeniť cez operátor priradenia.
### Operator priradenia

Operátor priradenia (`=`) sa používa na priradenie hodnoty premennej. Hodnota na pravej strane operátora sa priradí premennej na ľavej strane.

### Aritmetické operátory a priorita

Aritmetické operátory ako sú `+`, `-`, `*` a `/` sa používajú na vykonávanie základných matematických operácií.

Priorita operácií:
1. Zátvorky `()`
2. Násobenie `*` a delenie `/`
3. Sčítanie `+` a odčítanie `-`

### Matematické funkcie a metódy

Matematické funkcie a metódy sú volané na výpočty alebo manipuláciu s číselnými dátami.

- **Volanie matematických funkcií**: Napríklad `Math.sin()`, `Math.cos()`, `Math.sqrt()` v jazyku C#.
- **Výpočet obsahu kruhu pri zadanom polomere**: $Obsah = \pi r^2$, kde $\pi$ je matematická konštanta a $r$ je polomer kruhu :
```c#
using System;

static void Main(string[] args)
        {
            double polomer = 5;
            double obsah = Math.PI * Math.Pow(polomer, 2); //pi * r^2
            Console.WriteLine(obsah);
            Console.ReadKey();
        }
```