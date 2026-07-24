[← Letecká navigace](../05-letecka-navigace.html#bod-5){: .drobecek}

# GPS — princip, zobrazení, použití

*Detail k dalšímu studiu*

## Jak GPS funguje

**GPS (Global Positioning System)** je družicový navigační systém: kolem Země obíhá soustava družic, z nichž každá nepřetržitě vysílá signál s přesným časem (atomové hodiny) a svojí polohou. Tvůj přijímač měří, **jak dlouho signál letěl**, a z toho vypočte vzdálenost ke každé viditelné družici. Ze vzdáleností k **nejméně čtyřem družicím** pak určí svou polohu — tři na souřadnice (šířka, délka, výška), čtvrtá na opravu vlastních nepřesných hodin.

Klíčové vlastnosti:

- Přijímač je **pasivní** — jen poslouchá, nic nevysílá. Družice neví, kde jsi.
- Poloha se počítá na elipsoidu **WGS-84**.
- Vedle amerického GPS existují i další systémy (evropské **Galileo**, ruský GLONASS, čínský BeiDou) — moderní přijímače (souhrnně **GNSS**) je kombinují, což zlepšuje přesnost a spolehlivost.

## Co ti přístroj zobrazuje

- **Poloha** — souřadnice, poloha na mapovém podkladu.
- **Tracklog** — záznam celé trati letu. Dnes standard: rozbor letu doma, dokládání přeletů (XContest), i zpětné vyhodnocení, kudy vedla stoupání.
- **Groundspeed** — **rychlost vůči zemi**. Tohle vario bez GPS neumí! Porovnáním groundspeed s odhadem rychlosti vůči vzduchu poznáš vítr: letíš-li trimem (cca 38 km/h) a GPS ukazuje 20 km/h, máš protivítr kolem 18 km/h.
- **Track (traťový úhel)** — skutečný směr letu vůči zemi; spolu se šipkou k cíli (bearing) a vzdáleností tvoří základ navigace k bodu.
- **Výška GPS** — viz níže.

## GPS výška vs. barometrická výška

> **GPS vs. barometrická výška:** GPS měří výšku **geometricky** (z družic, vůči elipsoidu WGS-84) — chyba typicky v jednotkách až desítkách metrů, ale nezávisí na počasí. Barometrický výškoměr měří **tlak vzduchu** — krátkodobě jemnější a citlivější (proto vario pracuje s tlakem), ale závisí na správném nastavení a na změnách tlaku během dne.

Praktický důsledek: oba údaje se běžně liší i o desítky metrů a **není to porucha**. Pro srovnávání s výškovými hranicemi prostorů a s údaji v letectví je rozhodující **barometrická výška** — letecký provoz je celý postaven na tlakovém měření.

## Limity GPS — proč to není samospásné

- **Baterie a mráz:** vybitý přístroj nebo mobil zhasnutý mrazem ve výšce = konec navigace. Měj zálohu a mapu v hlavě.
- **Výpadek či rušení signálu:** vzácné, ale možné (terén, rušičky). 
- **Displej tě táhne do kabiny:** kdo v termice civí na displej, nekouká po ostatních kluzácích. Hlava venku, displej jen kontrolně.
- **GPS ti řekne, kde jsi — ne, kam smíš.** Bez nahrané aktuální mapy prostorů tě klidně navede nejkratší cestou skrz CTR. Aktuálnost prostorů ověřuj (AisView).

**Závěr instruktora:** GPS je skvělý pomocník a pro přelety dnes nezbytnost, ale základem zůstává **srovnávací navigace** — mapa, oči a přehled o terénu.

## Otázky k procvičení

<details>
<summary>Kolik družic potřebuje GPS přijímač k určení polohy a proč?</summary>
<p>Nejméně čtyři — tři na výpočet trojrozměrné polohy (šířka, délka, výška) a čtvrtou na opravu nepřesných hodin přijímače.</p>
</details>

<details>
<summary>Jak pomocí GPS odhadneš za letu sílu větru?</summary>
<p>Porovnáním rychlosti vůči zemi (groundspeed z GPS) s rychlostí kluzáku vůči vzduchu. Letím-li trimem cca 38 km/h a GPS ukazuje 20 km/h, mám protivítr zhruba 18 km/h; po větru by groundspeed byl naopak vyšší.</p>
</details>

<details>
<summary>Proč se GPS výška liší od výšky na barometrickém výškoměru a která platí vůči prostorům?</summary>
<p>GPS měří výšku geometricky vůči elipsoidu WGS-84, výškoměr měří tlak vzduchu závislý na nastavení a počasí — rozdíl desítek metrů je normální. Pro srovnávání s výškovými hranicemi prostorů je rozhodující barometrická výška.</p>
</details>

[← Zpět na Leteckou navigaci](../05-letecka-navigace.html#bod-5){: .btn-zpet}
