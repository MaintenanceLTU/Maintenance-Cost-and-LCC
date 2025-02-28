Bakgrund
========

I denna uppgift ska du genomföra en Life Cycle Cost (LCC)-analys av en
krossanläggning. Anläggningen består av en kross, en transportör och en
sikt anpassad för önskad kornstorlek. Du är ansvarig för denna
produktionsanläggning och ska undersöka hur olika faktorer påverkar din
LCC.

Handledningar för MATLAB och Python finns tillgängliga:
- [MATLAB Tutorial](../MATLAB/Maintenance_Cost_Analysis_MATLAB.md)  
- [Python Tutorial](../Python/Maintenance_Cost_Analysis_Python.md) 

Inkludera din kod som bilaga i rapporten.

Tillgänglighet och LCC-beräkningar
==================================

Tillgänglighetsberäkningar
--------------------------

Beräkna underhållstid och tillgänglighet med följande data:

-   **Kalkylränta:** 10%.

-   **Kalkylperiod:** 5 år.

-   **Drifttid:** 8 424 timmar per år (24 timmar/dygn, exklusive ett två
    veckors underhållsstopp i augusti).

-   **Avhjälpande underhåll:**

    -   Antal fel per år: 28.

    -   Medelreparationstid (MTTR): 0,8 dagar.

    -   Medelväntetid för avhjälpande underhåll: 0,2 dagar.

Presentera följande variabler i en tabell:

-   Förebyggande underhållstid

-   Reparationstid

-   Avhjälpande underhållstid

-   Otillgänglig tid

-   Tillgänglig tid

-   Operativ tillgänglighet ($A_o$)

Livscykelkostnadsberäkningar
----------------------------

Beräkna livscykelkostnaderna för anläggningen.

-   Årlig underhållskostnad.

    -   Medelkostnad per timme för avhjälpande underhåll: **7 000 SEK**.

    -   Kostnaden för det två veckors förebyggande underhållet: **1 400
        000 SEK**.

-   Årlig inkomst.

    -   Kapaciteten för krossanläggningen är **265 000 ton/år**.

    -   Priset för makadam är **100 SEK/ton**.

    -   Inkludera parametrar för:

        -   Anläggningseffektivitet (initialt satt till 1, full
            kapacitet).

        -   Kvalitet (initialt satt till 1, 100% kvalitetsutbyte).

-   Årliga driftskostnader:

    -   Energikostnad: 600 SEK/timme (påverkas av
        anläggningseffektivitet).

    -   Operatörskostnad: 500 SEK/timme.

-   Investeringskostnad: **14 000 000 SEK**.

-   Restvärde: Investeringen minskar med **50% per år**.

Beräkna nuvärde och nettonuvärde
--------------------------------

Beräkna nuvärde av årliga kostnader (drift, underhåll och inkomst) och
enstaka värden (restvärde). Beräkna sedan nettonuvärdet NNV och
rapportera enligt **Tabell [1](#NPVtable)**.

### **Table 1: Nuvärdersberäkning** <a id="NPVtable"></a>

| **Post**         | **Nuvärde**      | **Årligt belopp**  | **Belopp år X**      |
|------------------|------------------|--------------------|----------------------|
| Investeringskostnad | -XXX             |                    |                   |
| Underhållskostnad   | -XXX             | -XXX               |                   |
| Driftkostnad     | -XXX             | -XXX               |                      |
| Inkomst          | XXX              | XXX                |                      |
| Restvärde        | XXX              |                    |  XXX                 |
| **NNV**          | **XXX**          |                    |                      |



Förbättrad tillgänglighet
=========================

Ökad MTBF
---------

Utför samma beräkningar som i Uppgift 1 men med möjlighete att investera
i ökad MTBF.

-   Varje 1% extra MTBF ökar investeringskostnaden med **125 000 SEK**.

-   Lägg till '*PercentIncreasedMTBF*' och uppdatera antal fel och
    investeringskostnad.

    -   Tips: 10% ökad MTBF kan implementeras som 1/(1.10) minskade
        antal fel.

-   Beräkna **NNV för 10% ökad MTBF** och rapportera enligt samma tabellformat (Table [1](#NPVtable)).

Förebyggande underhållsstopp
----------------------------

Inkludera kortare **förebyggande underhållsstopp** i beräkningarna:

-   Varje kortare FU-stopp varar i **24 timmar**, kostar **140 000
    SEK**, och minskar antalet fel med **5%**.

-   Lägg till '*NumberOfShortPM*' och uppdatera antal fel, FU-tid och
    underhållskostnader.

-   Beräkna **NNV för 6 extra FU-stopp** och rapportera enligt samma tabellformat.

Optimering av underhåll
=======================

Optimalt antal % MTBF-ökningar
------------------------------

Plotta **NNV mot ökad % MTBF** i intervallet **0--100%** i steg om
**1%**, med **6 extra FU-stopp**.

Optimalt antal FU-stopp
-----------------------

Plotta **NNV mot antal FU-stopp** i intervallet **0--24 stopp**, med
**10% ökad MTBF**.

**Rapport:** Presentera optimal lösning och grafer.

Känslighetsanalys
=================

Genomför känslighetsanalys med **10% ökad MTBF och 6 extra FU-stopp**.

Minsta kvalitetsutbyte
----------------------

Sätt anläggningseffektiviteten till 95%. Vilket är det minsta
kvalitetsutbytet för att få ett positivt NNV?

Lönsamhetsgräns
---------------

Sätt anläggningseffektiviteten till 95% och kvaliteten till 95%. Vid
vilket makadampris blir NNV negativt?

Räntans påverkan
----------------

För ett makadampris på 85 SEK, vid vilken kalkylränta blir NNV $<0$?
Behåll anläggningseffektiviteten på 95% och kvaliteten på 95%.

**Rapport:** Presentera resultat och grafer.
