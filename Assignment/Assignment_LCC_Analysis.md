Background
==========

In this assignment, you are required to perform a Life Cycle Cost (LCC)
analysis of a crushing plant. The plant consists of a crusher unit, a
conveyor, and a screen adapted for the desired grain size. You are
responsible for this production facility and should investigate how
various factors affect your LCC.

Tutorials for MATLAB and Python are available
- [MATLAB Tutorial](../MATLAB/Maintenance_Cost_Analysis_MATLAB.md)  
- [Python Tutorial](../Python/Maintenance_Cost_Analysis_Python.md) 

Include your code ass appendix to your report.

Availability and LCC calculations
=================================

Availability Calculations
-------------------------

Calculate the maintenance time and availability using the following
data:

-   **Discount rate:** 10%.

-   **Calculation period:** 5 years.

-   **Operating time:** 8,424 hours per year (24 hours/day, excluding a
    two-week annual maintenance stop in August).

-   **Corrective maintenance:**

    -   Number of failures per year: 28.

    -   Mean Time to Repair (MTTR): 0.8 days.

    -   Mean Waiting Time for Corrective Maintenance: 0.2 days.

Present the following variables in a table:

-   Preventive maintenance time

-   Repair time

-   Corrective maintenance time

-   Downtime

-   Available time

-   Operational availability ($A_o$)

Life Cycle Cost Calculations
----------------------------

Calculate the life cycle costs of the asset.

-   Yearly maintenance cost.

    -   The mean hourly cost for corrective maintenance is **7,000
        SEK**.

    -   The cost of the two-week preventive maintenance cost is
        **1,400,000 tons/year**.

-   Yearly income.

    -   The capacity of the crusher plant is **265,000 tons/year**.

    -   The price of macadam is **100 SEK / ton**.

    -   Include parameters for:

        -   Performance (initially set to 1, full capacity).

        -   Quality (initially set to 1, 100% quality yield).

-   Yearly operating costs:

    -   Energy cost: 600 SEK/hour (scalable with performance).

    -   Operator cost: 500 SEK/hour.

-   Investment cost:

    -   The basic price of the asset is **14,000,000 SEK**.

-   Residual value:

    -   Investment reduces by **50% per year**.

## Calculate Present Values and NPV  

Calculate present values of annual costs (operation, maintenance, and income) and single amounts (residual value). Then compute NPV and report using the table format in **Table [1](#NPVtable)**.

### **Table 1: NPV Calculation Summary** <a id="NPVtable"></a>

| **Item**          | **Present Value** | **Annual Amounts** | **Amount in Year X** |
|------------------|------------------|--------------------|----------------------|
| Investment Cost  | -XXX             |                    |                      |
| Maintenance Cost | -XXX             | -XXX               |                      |
| Operating Cost   | -XXX             | -XXX               |                     |
| Income          | XXX              | XXX                |                      |
| Residual Value  | XXX              |                    |  XXX                 |
| **NPV**          | **XXX**          |                    |                      |



Improving availability
======================

Increasing MTBF
---------------

Perform the same calculations as in Task 1, assuming an additional MTBF.
Each **1% extra MTBF** increases the investment cost by **125,000 SEK**.
Compute the **NPV for 10% extra MTBF** using the same table format
(Table [1](#NPVtable)).

**Tip:** A 10% increase in MTBF is modeled as a **$1/(1.10)$ reduction**
in the failure rate.

Preventive Maintenance Stops
----------------------------

Perform the same calculations but include **preventive maintenance (PM)
stops**:

-   Each PM stop lasts **24 hours**, costs **140,000 SEK**, and reduces
    failures by **5%**.

-   Update failure count, PM time, and maintenance costs.

Compute NPV for**6 additional PM stops** and report using the same table
format.

Maintenance Optimization
========================

Finding Optimal MTBF Increase
-----------------------------

Plot **NPV vs. extra % MTBF** for the range **0--100%**, in **1%
steps**, using **6 extra PM stops**.

Finding Optimal PM Stops
------------------------

Plot **NPV vs. number of PM stops** in the range **0--24 stops**, using
**10% extra MTBF**.

**Report:** Present the optimal solution with graphs.

Sensitivity Analysis
====================

Perform sensitivity analysis using **10% extra MTBF and 6 extra PM
stops**.

Minimum Quality Yield
---------------------

Set plant efficiency to 95%. What is the minimum quality yield needed
for a positive NPV?

Break-even Price
--------------------

Set plant efficiency to 95% and quality to 95%. At what crushed stone
price does NPV become negative?

Interest Rate Sensitivity
-------------------------

For a **stone price of 85 SEK**, what discount rate causes NPV $<0$?

**Report:** Present results and graphs.
