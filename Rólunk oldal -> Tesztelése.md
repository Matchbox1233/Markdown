## 1. Tesztterv

1. Menüsor tesztelés
    * Az egér mutató hatására milyen stílsú lesz az adott gomb a menüsoron. Az adott menü gombok megfelelő oldalakra mutatnak e, illetve a navigációs menü reszponzivitása különböző méretű készülékekre.
    
2. Cím és alcím tesztelése
    * A cím és alcím reszponzivitásának ellenőrzése különböző szélességű készülékeken.

3. A menüsor és a cím borítóképének tesztelése
    * Ellenőrizzük a kép méretének arányos növekedését vagy csökkenését az adott eszköz méretéhez, így ellenőrizzük a reszponzivitását. A borító megfelelő helyzetben marad e a méretnövekedésne köszönhetően.

4. Bal oldali kör alakú képek tesztelése
    * Méretváltozás esetén ellenőrizzük, hogy a képek megtartják e az adott helyüket. A kisebb képernyők esetében alkalmazkodnak e az új mérethez (segítik e a felhasználó tájékozódását mobil eszközökön is, tehát nem takarnak ki szöveget és nem lesznek túl nagyok). MIndig a bal oldalon kell lenniük, kivéve ha a méretcsökkenés megköveteli a helyes átrendeződést.
    
5. Jobb oldali kör alakú képek tesztelése
    * Méretváltozás esetén ellenőrizzük, hogy a képek megtartják e az adott helyüket. A kisebb képernyők esetében alkalmazkodnak e az új mérethez (segítik e a felhasználó tájékozódását mobil eszközökön is, tehát nem takarnak ki szöveget és nem lesznek túl nagyok). Mindig kisebbnek és a jobb oldal kell lenniük, kivéve ha a méretcsökkenés megköveteli a helyes átrendeződést.

6. Bekezdés címek tesztelése
    * Ellenőrizzük a bekezdés címeket, hogy az adott méretváltozásra helyesen váltanak méretet, főként a mobil eszközökre. Az olvashatóság és a weboldal könnyű használata miatt. A cím ne takajon el szöveget illetve ne csússzon el az oldalon méretváltoztatás miatt.
    
7. Bekezdések tesztelése 
    * Megnézzük a bekezdések reszponzivitását. Az ablak méretének csökkenésével tudjuk ellenőrizni, hogy adott méretekben, a szöveg nem lóg e bele a képekbe, valamint helyesen lesz e törrdelve.
    
8. Elválasztó vonal tesztelése
    * A vonal mindig a bekezdések alatt és a lábrész felett helyezkedik el. Megnézzük, hogy a vonal nem csúszik e el, vagy, hogy végig ér az adott oldalon különböző méretek mellett.

9. Elérhetőség tesztelése
    * Az ikonoknak mindig a z adott sor előtt kell állniuk, minden méret esetén. Valamint a szövegnek is igazodnia kell a kijelző méretekhez.
    
10. Fedezze fel a szolgáltatásainkat tesztelése 
    * Cím és a szöveg, valamint az egész blokk helyzetének az igazodása. Minden esetben cím, bekezdés, és alatta pedig a gombot kell látnunk oszlopszerűen. Ellenőrizzük a "oszlop" minden elemének reszponzivitását. A gomb stílusának helyessége minden esetben és a helyes oldara továbbításának az ellenőrzése.
    
11. Lépjen kapcsolatba velünk tesztelése
    * A szövegdobozok méretének és helyzetének ellenőrzése, valamint a felszólító üzenet helyessége minden méret esetén. A gomb stílusa és reszponzivitása.

12. Social links tesztelése
    * A szövegrész és a vonal sítlusának ellenőrzése minden képrenyő mérethez a  helyzetük megtartásával 
    
13. Social ikonok tesztelése
    * Az ikonok animációjának tesztelése minden méretben, illetve az ikonok elhelyezése a hátterükön megfelelő e.
    
14. Terms | privacy tesztelése
    * Ellenőrizzük a két szó helyzetét és stílusát minden képernyőhöz.   
    
    
## 2. Felkészülés a végrehajtásra

A teszteléshez használt eszközök/programok:
* Visual Studia Code
    * Live Server bővítmény (nem kötelező)
* Általunk kedvelt böngésző (Internet Explorer nem ajánlott)

A tesztek Windows-os környzetben készültek.


## 3. Tesztek Végrehajtása

> 1. Menüsor tesztelés
>    * Az egér mutató hatására milyen stílsú lesz az adott gomb a menüsoron. Az adott menü gombok megfelelő oldalakra mutatnak e, illetve a navigációs menü reszponzivitása különböző méretű készülékekre.

**A navigációs menüsor alapesetben:**
![Navbar alap állpota](/Images/Navbar1.png "Navbar alap állpota")

**A navigációs menüsor aktív kurzor esetén:**
![Navbar állpota aktív kurzor esetén](/Images/Navbar2.png "Navbar állpota aktív kurzor esetén")

*A fenti két képen jól látszik a különbség. Amíg csak alap esetben van a navigációs sor, addig minden menüpont ugyanúgy jelenik meg, tehát nincs méretbeli és színbeli eltérés. De amikor rávisszük az egeret valamelyik menüpontra, akkor az kiemelkedik, a többi menü addig halványabbá válik. Látszódik rajta egy animáció a kattintás előtt.

**Menüpontok beállításai a megfelelő oldalakra:**

    <ul>
      <li><a href="../forum.php">Fórum</a></li>
      <li><a href="../kapcsolat_oldal/kapcsolat.html">Kapcsolat</a></li>
      <li><a href="../szolgaltatasok_osszessege_weboldal/szolgaltatasok.html">Szolgáltatások</a></li>
      <li><a href="../rounk_oldal/rolunk.html">Rólunk</a></li>
      <li><a href="../belepes.php">Belépés</a></li>
      <li><a href="../regisztracio.php">Regisztráció</a></li>
     </ul>

*A fenti kódrészletben láthatjuk a menüsor forrásának egy részét. Itt határozzuk meg, hogy melyik menüpont melyik oldalra visz minket. Mint láthatjuk minden gomb a hozzá tartozó oldalra mutat. Minden oldal külön mappában található, az egyértelműség miatt.

Menüsor reszponzivitása 1920px szélesség esetén:

![Navbar reszponzivitása 1920px](/Images/Navbar3.png "Navbar reszponzivitása 1920px")

Láthatjuk, hogy a menüsor teljesen használható, nem csúszik el, nem megy össze. Pontosan a helyén marad.

Menüsor reszponzivitása 960px szélesség esetén:

![Navbar reszponzivitása 960px](/Images/Navbar4.png "Navbar reszponzivitása 960px")

![Navbar reszponzivitása 960px](/Images/Navbar5.png "Navbar reszponzivitása 960px")

Láthatjuk, hogy a navigációs sor eltűnt és csak egy gomb van a helyén (első kép). A gomb nyomása esetén bal oldalt felbukkan a menüsor (második kép) csak most már oszlopos alakban, nem pedig sorban. Ezzel a módszerrel könnyen alkalmazkodhatunk különböző kijelzőkhöz is, mint például a mobil kijelzők. Ebben az esetben is érvényesül, hogy a menüsor minden pontja látszik, de ha rávisszük az egyik pontra az egeret, akkor az adott pont kiemelkedik, létrejön az animáció. A többi gomb pedig addig elhalványul.

Menüsor reszponzivitása mobilon:

![Navbar reszponzivitása mobilon](/Images/Navbar6.png "Navbar reszponzivitása mobilon")

Ebben az esetben is látszik, hogy a bal oldalon az oszlopos elrendezésben vannak a menüpontok. Ezt a módszert alkalmaztuk az 1200px vagy attól kisebb szélességű kijelzők esetén.
