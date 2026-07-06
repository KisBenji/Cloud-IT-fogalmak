# Cloud-IT-fogalmak
## Skálázás, terheléselosztás, hibatűrés
A legkedvesebb témakör az alapfogalmak közül **terheléselosztás (load balancing)** és a **skálázás (scaling)**  fontossága, hogy a rendszer kapacitása igény szerint csökkenthető/növelhető akár a megnövekedett forgalom/felhasználók száma miatt vagy legyen szó napszakos vagy szezonális terhelésről vagy az üzleti igények bővülésével több feladatot ellátó szervernek a skálázása. Úgy tudjuk támogatni a fejlődést, hogy alapjában véve nem kell teljesen új rendszert tervezni. 
Ezek közül a két leginkább alapvető megoldás: 

*1. Vertikális skálázás* a szerver gép teljesítmény növelése (CPU,RAM).

*2. Horizontális skálázás* több gép bevonása párhuzamosan, elosztva a terhelést.

Ami ebben a legjobban tetszik az előretervezés és tudatos felépítése az infrastruktúrának, hogy egyszerre legyen magas rendelkezésreállás **(HA)** és olyan tartalék elemek bevonása, amely egy hiba esetén is a szerver biztonságos működését támogatja **(redundancia)**. Ezeknek a rendszereknek a tudatos megépítése javítja a felhasználói élményt, javítja a válaszidőt miközben az erőforrásokat hatékonyan használjuk ki. Ezt lehet kiegészítni olyan biztonsági elemekekkel még, mint a hibatűrő vagy **fault tolerance**, ahol egy-egy komponens kiesése mellett is tovább tud működni a rendszer. 
