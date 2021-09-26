# Funkcionális specifikáció

## Áttekintés

- A fejlesztésünk célja, egy olyan weboldal elkészítése, mellyel képesek leszünk nyilvántartani autók adatait, és internetes vásárlást biztosítani.
- A rendszer célja a könnyű kezelhetőség és átláthatóság. Bárki számára gyorsan és egyszerűen megtanulható legyen.
- Az autók megvásárlása regisztrációhoz van kötve, böngészni viszont lehet nélküle is.
- Az aktuális vásárlások kilistázására is lesz lehetőség.
- A weboldal tartalmazni fog képeket, elérhetőségeket és az ehhez szükséges információkat.

## Jelenlegi helyzet

- A mai világban már elengedhetetlen, hogy szoftveresen is vezetve legyenek az adminisztrációs dolgok. Ezért szükség van egy olyan weboldalra, ami segít könnyebben tájékozódni a vásárlások, pénzösszegek és a vevő igényei között. Ezáltal visszakövethetőbbé is teszi ezt.

- A jelenlegi helyzet, hogy papíron, jegyzetben van vezetve, ami nagyon lassú ahhoz, hogy a vevők igényei ki legyenek elégítve. Ezt pedig nehéz úgy kivitelezni, hogy az alkalmazottaknak kevesebb idejük marad más teendőkre.

- Muszáj a pénzösszegek kezelését is egyszerűbbé tenni. Jelenlegi formában ez nehéz, és nehezen nyomon követhető. Sok időt vesz igénybe a dokumentumok, papírok karbantartása, tárolása. Nem egyszerű több évre visszamenőleg keresni.

## Követelménylista
| modul | id | név | verzió | kifejtés |
|--|--|--|--|--|
| funkció | F1  | Listázás| 1.0 |Ki lehessen listázni a rendelkezésre álló autókat. Ehhez nem szükséges fiókkal rendelkeznünk az oldalon, de a vásárláshoz már igen.
|funkció| F2| Vásárlás | 1.0 | Legyen lehetőség az elérhető autók megvásárlására fiókkal rendelkező felhasználók számára.
| funkció | F3 | Fiókok lekérdezése | 1.0 | Itt tudjuk lekérni a regisztrált fiókok adatait (Adminisztrátor, alkalmazott, vásárló).


## Jelenlegi üzleti folyamatok modellje
Néhány használtautó-kereskedés a mai napig a hagyományos, papír alapú módszert használja a rendelések, leltár számontartásához. Az alkalmazott a rendelési adatokat egy jegyzőkönyvbe/naptárba rögzíti.
 Ennek számos hátránya van:
 - Lassan és nehezen átlátható rendszer
 - Megrendelők adatai összekeveredhetnek
 - Hiba kockázat az adatok feljegyzésekor
 - Az egész dokumentáció elveszhet
 - Számla kiállítása körülményes
 - Nem környezetbarát módszer

## Igényelt üzleti folyamatok modellje

 - Weboldalunk célja, hogy leegyszerűsítsük egy autókereskedés elérhető autóinak és megrendeléseinek kezelését a papír alapú munkához képest. Csökken a hibalehetőségek száma is.
 - Célunk, hogy bármely elérhető autó megvásárolható legyen regisztrált felhasználók számára.
 
## Használati esetek

Az autókereskedés alkalmazottja[i] kezeli[k] a rendszert, ami azt jelenti, hogy a használati esetek többsége hozzá[juk] kapcsolódik. Az adminisztrátor[ok] emelt jogosultsággal rendelkezik/rendelkeznek, a felhasználók hozzá[juk] fordulhatnak speciális esetekben.

Adatbázisban lévő adatok kezelése:
- Adatok hozzáadása, törlése, módosítása.

## Megfeleltetés, hogyan fedik le a használati esetek a követelményeket 

Az alkalmazotti feladatkör ellátja a szervezési feladatokat (autók felvitele, rendelések kezelése). A weboldal megnyitásakor megnyílik a főoldalunk, ahol található a navigációs sáv, ahol a felhasználó ki tudja választani az autók menüpontot és azon belül a tetszőleges autót amit meg kíván nézni/vásárolni. Egy autóra kattintva előhozhatjuk az autó adatait, ahol megtalálhatjuk a “Megrendelem” gombot amely egy újabb formra irányít minket ahol a mezők kitöltése után meg tudjuk vásárolni a kiválasztott autót. De található még három, a vásárló számára nem látható menüpont is a főoldalon. Egy Feltöltés menüpont, ahol új autót tudunk feltölteni, egy Módosítás menüpont, ahol az autók adatait lehet módosítani, illetve egy Rendelés státuszok menüpont, ahol lehetőség van a rendelések státuszainak a módosítására, valamint egy Vásárlások menüpont, ahol egy excel táblázatként tudjuk letölteni az eddigi vásárlások adatait.

>>>>>>> 4ffe125b6be5f2ea98b1f6679ed8fa839a34193e
