Bakgrund {#bakgrund .unnumbered}
========

I denna uppgift ska du genomföra en Life Cycle Cost (LCC)-analys av en
krossanläggning. Anläggningen består av en kross, en transportör och en
sikt anpassad för önskad kornstorlek. Du är ansvarig för denna
produktionsanläggning och ska undersöka hur olika faktorer påverkar din
LCC.

Handledningar för MATLAB och Python finns tillgängliga, besök:
[MaintenanceLTU GitHub
Repository](https://github.com/MaintenanceLTU/D0002B/tree/main/Maintenance%20Cost%20and%20LCC).
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

Förbättrad tillgänglighet
=========================

Ökad MTBF
---------

Utför samma beräkningar som i Uppgift 1 men med en ökad MTBF. Varje **1%
extra MTBF** ökar investeringskostnaden med **125 000 SEK**. Beräkna
**NPV för 10% extra MTBF** och använd samma tabellformat.

Förebyggande underhållsstopp
----------------------------

Inkludera **förebyggande underhållsstopp** i beräkningarna:

-   Varje FU-stopp varar **24 timmar**, kostar **140 000 SEK**, och
    minskar antalet fel med **5%**.

-   Uppdatera felantal, FU-tid och underhållskostnader.

Beräkna **NPV för 6 extra FU-stopp** och använd samma tabellformat.

Optimering av underhåll
=======================

Optimalt antal MTBF-ökningar
----------------------------

Plotta **NPV mot extra % MTBF** i intervallet **0--100%** i steg om
**1%**, med **6 extra FU-stopp**.

Optimalt antal FU-stopp
-----------------------

Plotta **NPV mot antal FU-stopp** i intervallet **0--24 stopp**, med
**10% extra MTBF**.

**Rapport:** Presentera optimal lösning och grafer.

Känslighetsanalys
=================

Genomför känslighetsanalys med **10% extra MTBF och 6 extra FU-stopp**.

Minsta kvalitetsutbyte
----------------------

Sätt anläggningseffektiviteten till 95%. Vilket är det minsta
kvalitetsutbytet för att få ett positivt NPV?

Lönsamhetsgräns
---------------

Sätt anläggningseffektiviteten till 95% och kvaliteten till 95%. Vid
vilket makadampris blir NPV negativt?

Räntans påverkan
----------------

För ett makadampris på 85 SEK, vid vilken kalkylränta blir NPV $<0$?
Behåll anläggningseffektiviteten på 95% och kvaliteten på 95%.

**Rapport:** Presentera resultat och grafer.
