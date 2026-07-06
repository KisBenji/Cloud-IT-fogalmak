# Cloud-IT-fogalmak
## Skálázás, terheléselosztás, hibatűrés
A legkedvesebb témakör az alapfogalmak közül **terheléselosztás (load balancing)** és a **skálázás (scaling)**  fontossága. Ezt a témakört már érintettem a gyakorlatban is, hoztam létre virtuális szervert Azure-ben és terheléselosztót integráltam, hogy a rendszer kapacitása igény szerint csökkenthető/növelhető legyen akár a megnövekedett forgalom/felhasználók száma miatt vagy legyen szó napszakos vagy szezonális terhelésről vagy az üzleti igények bővülésével több feladatot ellátó szervernek. Úgy tudjuk támogatni a fejlődést, hogy alapjában véve nem kell teljesen új rendszert tervezni. 
Ezek közül a két leginkább alapvető megoldás: 

*1. Vertikális skálázás* a szerver gép teljesítmény növelése (CPU,RAM).

*2. Horizontális skálázás* több gép bevonása párhuzamosan, elosztva a terhelést.

Ami ebben a legjobban megtetszett az az előretervezés és tudatos felépítése az infrastruktúrának, hogy egyszerre legyen magas rendelkezésreállás **(HA)** és olyan tartalék elemek bevonása, amely egy hiba esetén is a szerver biztonságos működését támogatja **(redundancia)**. Ezeknek a rendszereknek a tudatos megépítése javítja a felhasználói élményt, javítja a válaszidőt miközben az erőforrásokat hatékonyan használjuk ki. Ezt lehet kiegészítni olyan biztonsági elemekekkel még, mint a hibatűrő vagy **fault tolerance**, ahol egy-egy komponens kiesése mellett is tovább tud működni a rendszer. Sokszor lehet találkozni olyan oldalakkal, ahol terheléselosztás és a skálázás fontosságát kihagyva az oldal felépítésére fokúszáltak, majd egy hirtelen megnövekedett forgalom esetén az oldal elérhetetlen lesz perceken belül. 

Ha az AWS terheléselosztó megoldásokat akarjuk kicsit bővebben megismerni, akkor a [https://aws.amazon.com/elasticloadbalancing/application-load-balancer/] linket böngészve tudjuk megtenni. 🙂
