a)
1. Uveďte, na čo slúžia funkcie a metódy a aký je medzi nimi rozdiel
2. Charakterizujte parametre, uveďte konkrétne príklady parametrov
3. Uveďte, ako sú volané funkcie a metódy bez návratovej hodnoty a ako s návratovou hodnotou
4. Vysvetlite, čo rozumieme pod preťažovaním funkcií a metód
5. Vysvetlite, čo rozumieme pod predefinovaním metód
b)
1. Vysvetlite, aký je rozdiel medzi statickými a nestatickými metódami
2. Vymenujte modifikátory prístupu v objektovom programovaní a uveďte, aký je medzi nimi rozdiel
3. Vytvorte program s dvomi triedami: jednu s metódou Main() a druhú s dvomi metódami – statickou na výpočet aritmetického priemeru piatich celých čísel a nestatickou na zistenie počtu slov vo vete
c)
1. Zdôvodnite potrebu protokolu ARP
2. Vysvetlite úlohy a postavenie NBS, ktorá je súčasťou eurosystému
3. 

---

1. **Parametre**
   - Parameter metódy udáva aký typ hodnoty musí užívateľ zadať pri volaní metódy. Parametre majú aj pomenovanie s ktorým sa pracuje v metóde ako hodnotami. Pri volaní metódy užívateľ odovzdáva metóde argumenty, ktoré musia spĺňať parametre ako je dátovy typ ale môžu niesť iný názov.

2. **Volanie funkcií a metód bez návratových hodnôt a s návratovými hodnotami**
   - Funkcie a metódy môžu byť volané s cieľom vykonávať určité úlohy alebo manipulovať s dátami. Niektoré z nich môžu vrátiť hodnotu po vykonaní, zatiaľ čo iné môžu byť použité len na vykonanie určitých akcií bez návratu žiadnej hodnoty.

3. **Preťažovanie funkcií a metód**
   - Preťažovanie funkcií a metód je proces, kde viacero funkcií alebo metód má rovnaký názov, ale rôzne parametre. To umožňuje programátorovi vytvárať flexibilné a jednoducho použiteľné funkcie/metódy s rôznymi typmi vstupných dát.

4. **Predefinovanie funkcií a metód**
   - Predefinovanie, tiež známe ako prepísanie, je koncept v OOP, ktorý umožňuje podtriede (dedičnej triede) poskytnúť vlastnú implementáciu metódy, ktorá už bola definovaná v nadtriede. Tým sa mení správanie metódy v podtriede podľa potreby.

5. **Rozdiel medzi statickými a nestatickými metódami**
   - Statické metódy sú priradené triede a nie konkrétnej inštancii objektu. Môžu byť volané priamo z triedy a nemajú prístup k inštancijným premenným. Naopak, nestatické metódy sú volané z konkrétnej inštancie triedy a môžu pristupovať k jej inštancijným premenným.

6. **Modifikátory prístupu v OOP**
   - Modifikátory prístupu v OOP určujú, kto môže pristupovať k členom triedy (premenným, metódam, getterom, setterom)
   - Tieto modifikátory sú: public, private, protected.
   - K public atribútom môžeme pristupovať priamo a dajú sa dediť.
   - Protected časti objektov: prístup k ním je utajený ale jeho atribúty môžu dediť triedy
   - Privátne časti objektu sú prístupné len k objektu.
   
7. **Program - v metóde Main() spraviť z inej triedy volanie statickej a nestatickej metódy**

```csharp
// main.cs
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace TCOZMS_OOP
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Trieda vec1 = new Trieda(20);
            Trieda vec2 = new Trieda(30);
            Console.WriteLine("Celkovo: " + Trieda.GetCelkovo());
            Console.WriteLine("Pocet vec1: " + vec1.GetPocet());
            Console.WriteLine("Pocet vec2: " + vec2.GetPocet());
            Console.ReadKey();
        }
    }
}

// trieda.cs
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace TCOZMS_OOP
{
    internal class Trieda
    {
        static int celkovo = 0;
        int pocet;

        public Trieda()
        {
            pocet = 0;
        }

        public Trieda(int poceet) {
            this.pocet += poceet;
            celkovo += this.pocet;
        }

        public static int GetCelkovo()
        {
            return celkovo;
        }

        public int GetPocet()
        {
            return this.pocet;
        }

        public void SetPocet(int pocet)
        {
            this.pocet = pocet;
        }
    }
}
```