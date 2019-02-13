# Colonization of Tomato Stem

**Written/Edited by**: Tiffany Lowe-Power, Madeline Hayes, Mandel lab

## Experimental Design:

* **Timing**:
    * *Colonization assays (e.g. comparing two strains) should be **sampled at specific time points** (will show delay(s) in colonization if time points are before population levels saturate) and not at specific symptom level (even if a strain takes longer to initiate symptoms, at symptom onset, plants will have ~5x10<sup>8</sup>-5x10<sup>9</sup> CFU/g)*
    * Growth curve after **tomato petiole inoculation**: 0, 1, 2, 3 dpi
    * Growth curve (stem) after **soil drench inoculation**: 4, 6, 8 dpi
        * Time 0 is not informative because bacteria are sampled into the soil and sampling is in the stem. 
        * Infection via soil-drench is stochastic. 4 dpi is probably the earliest you want to do, but even then, many plants will be uncolonized. 
        * Even though you will probably plan days 1-3 over a weekend, it is *crucial* to keep soil moisture level high during this window.
* **Sampling site**:
    * **Cut-Petiole**: Sample at the site of inoculation `'+0'`and a distal site (e.g. 3 cm above the site of inoculation `'+3'`).
        * After cut-petiole, the bacteria will first establish at the site of inoculation, then below the site of inoculation before establishing above the site of inoculation. 
        *This probably reflects connectivity of vascular architecture*
    * **Soil-Soak**: Sample at the cotyledon junction

## Plant Inoculation

Follow the [petiole](tomato_petiole_inoc.md) or [soil soak](tomato_ss_inoc.md) inoculation protocols

## Destructive Sampling of Stem

### Preparation

1. `CPG+TZC(+antibiotic) plates`: **1 per sampling site**; labeled for 10<sup>0</sup> to 10<sup>-7</sup> dilutions.
1. `Bead tubes`: **1 per sampling site**; filled with 4x 2.22 mm metal beads & 900 ul dI H2O;  
    * ***labeled on side**--powerlyzer rubs labels off top*
    * Can prepare up to 1 week in advance
1. Check consumable levels in advance: 
    * 200 ul tips (1 box per 12 samples) - autoclaved
    * 96-well **round-bottom** microplate (1 per 12 samples) - sterilized in 10% bleach 30 min, 4x thorough rinses with diH2O, dried in 50C oven... or new microplate.
1. Load microplate with di H2O to dilution plate samples
    * Pour di H2O into a sterile reservoir (autoclaved glass petri dish or  plastic petri dish).
    * Using multichannel P200, add 180 ul to 7 rows well of microplate (A-G). 

### Sampling

1. Use a razor blade to sample 100 mg +/- 10 mg stem. 
Record mass for normalization. 
    * *Sharps safety*: Discard dulled blades in *sharps trash*. 
    When cutting stem, especially of older lignified plants, be careful of hand placement with respect to cutting angle. 
1. Place plant stem in bead tube. 
Homogenization will be inefficient for biomass that does not move readily; cut large samples before homogenization. 
Repeat for 12-24 samples. 
1. Homogenize samples in batches of 12-24. 
*Verify lid is screwed on each tube as you load it*
    * *Powerlyzer program*: 2 rounds of 2200 rpm for 1.5 min each with 4 min rest (to minimize sample heating).
    * If you have multiple treatments (e.g inoculating strains) and will process in multiple batches, evenly spread out treatments between batches. 
    * *If you need to pause, it's best to pause before homogenization. 
    Homogenization will release nutrients that can promote bacterial growth before dilution plated.*  
1. After homogenization, inspect samples to verify complete homogenization. 
*Protip*: incompletely homogenized samples usually have less chlorophyll in suspension.
1. Dilute samples according to [dilution plating protocol](cfus.md). Finish homogenizing samples in batches of 12 or 24. 

## Data Analysis: 
* Copy calculations from [bacterial density workbook](workbooks/bacterial_density_workbook.xlsx) into a digital lab notebook entry and calculate CFU / g stem. 
* In GraphPad Prism, plot individual data points and medians on a logarithmic scale.
* The data are often not normally distributed, with different variances, and the outliers may contain biologically meaningfully information. 
Therefore, non-parametric tests provide a useful method to determine whether the treatments differ significantly.
* Use GraphPad Prism software or similar for statistical analysis. 
For two treatments, use the Wilcoxon Rank Sum test. 
For comparisons among greater than two treatments, use the Kruskal-Wallis test with appropriate post-tests for multiple comparisons. 
* *Recommendation*: Keep track of experiment throughout digital files with a timestamp on the inoculation day. 
e.g 20191231 (year, month, day is sequential *in computer* and compatible for US vs. International dating norms)