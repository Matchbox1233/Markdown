# Fitt oldal tesztelése


## 1. Tesztterv

1. Fejléc tesztelés
    * Az egér mutató hatására milyen stílsú lesz az adott gomb a menüsoron. Az adott menü gombok megfelelő oldalakra mutatnak e, illetve a navigációs menü reszponzivitása különböző méretű készülékekre. A cím arányosan nő illetve csökken a méretváltozásra. A fejléc hátterének reszponzicitása.
    
2. Fő rész tesztelés
    * A háttér, illetve a rajta lévő box helyzetének a változása. A gombok, választható opciók működése. A linkek és a felugró ablakok helyzete minden méret esetén. A gombok aktivitása kattintás esetén.
    
  
3. Lábrész tesztelés
    * A három oszlopos tagolás, a mezők helyzetet illetve a közzössségi oldalra vezető linkek helyzete és rezspozivitása, valamint ezek animációi minden méretben.


## 2. Felkészülés a végrehajtásra


A teszteléshez használt eszközök/programok:


* Visual Studia Code
    * Live Server bővítmény (nem kötelező)
* Általunk kedvelt böngésző (Internet Explorer nem ajánlott)


A tesztek Windows-os környzetben készültek.


## 3. Tesztek Végrehajtása

> ### **1. Fejléc tesztelés**
>    * Az egér mutató hatására milyen stílsú lesz az adott gomb a menüsoron. Az adott menü gombok megfelelő oldalakra mutatnak e, illetve a navigációs menü reszponzivitása különböző méretű készülékekre. A cím arányosan nő illetve csökken a méretváltozásra. A fejléc hátterének reszponzicitása.


**A fejléc alapesetben:**
![A fejléc alap állpota](/Images/Fejlec1.png "A fejléc alap állpota")

**A navigációs menüsor aktív kurzor esetén:**
![A fejléc állpota aktív kurzor esetén](/Images/Fejlec2.png "A fejléc állpota aktív kurzor esetén")


*A fenti két képen jól látszik a különbség. Amíg csak alap esetben van a navigációs sor, addig minden menüpont ugyanúgy jelenik meg, tehát nincs méretbeli és színbeli 
eltérés. De amikor rávisszük az egeret valamelyik menüpontra, akkor az kiemelkedik, a többi menü addig halványabbá válik. Látszódik rajta egy animáció a kattintás előtt.*


**Menüpontok beállításai a megfelelő oldalakra:**

    <ul>
      <li><a href="../forum.php">Fórum</a></li>
      <li><a href="../kapcsolat_oldal/kapcsolat.html">Kapcsolat</a></li>
      <li><a href="../szolgaltatasok_osszessege_weboldal/szolgaltatasok.html">Szolgáltatások</a></li>
      <li><a href="../rounk_oldal/rolunk.html">Rólunk</a></li>
      <li><a href="../belepes.php">Belépés</a></li>
      <li><a href="../regisztracio.php">Regisztráció</a></li>
     </ul>


*A fenti kódrészletben láthatjuk a menüsor forrásának egy részét. Itt határozzuk meg, hogy melyik menüpont melyik oldalra visz minket. Mint láthatjuk minden gomb a hozzá tartozó oldalra mutat. Minden oldal külön mappában található, az egyértelműség miatt.*


**A fejléc reszponzivitása 1920px szélesség esetén:**


![A fejléc reszponzivitása 1920px](/Images/Fejlec3.png "A fejléc reszponzivitása 1920px")


*Láthatjuk, hogy a menüsor teljesen használható, nem csúszik el, nem megy össze. Pontosan a helyén marad.*


**A fejléc reszponzivitása 960px szélesség esetén:**


![A fejléc reszponzivitása 960px](/Images/Fejlec4.png "A fejléc reszponzivitása 960px")


*Láthatjuk, hogy a navigációs sor eltűnt és csak egy gomb van a helyén (első kép). A gomb nyomása esetén bal oldalt felbukkan a menüsor (második kép) csak most már oszlopos alakban, nem pedig sorban. Ezzel a módszerrel könnyen alkalmazkodhatunk különböző kijelzőkhöz is, mint például a mobil kijelzők. Ebben az esetben is érvényesül, hogy a menüsor minden pontja látszik, de ha rávisszük az egyik pontra az egeret, akkor az adott pont kiemelkedik, létrejön az animáció. A többi gomb pedig addig elhalványul.*


**A fejléc reszponzivitása mobilon:**


![A fejléc reszponzivitása mobilon](/Images/Fejlec5.png "A fejléc reszponzivitása mobilon")


*Ebben az esetben is látszik, hogy a bal oldalon az oszlopos elrendezésben vannak a menüpontok. Ezt a módszert alkalmaztuk az 1200px vagy attól kisebb szélességű kijelzők esetén.*

