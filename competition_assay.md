# Bacterial competition assays

**Written/Edited by**: Tiffany Lowe-Power, 

## Experimental Design:
Note: This is the protocol where 2 strains are co-inoculated into a condition and allowed to competitively grow. For single-strain inoculations, see the [Stem colonization protocol](col_tomato_stem.md) or other assays. This protocol is written for tomoato plant assays, but you could develop in vitro or other in plant assays. 

* **Strains**: You must work with strains that are marked by different antibiotic resistance markers. Ultimately you will be dilution plating the mixture of strains on plates with 2 different antibiotics.  So they must have different resistance markers so that you can count each strain individually. If your strains are unmarked or marked with the same antibiotic, you should be able to use the MiniTn7 vectors to add a Gentamicin (Ec61) or Kanamycin resistance cassette (Ec71) into the chromosome. When transforming the Tn7 plasmids into your strain, don't forget to co-transform with a helper plasmid (pTNS2 or pTNS3)
    * **Best practice**: In case the antibiotic cassettes confer a fitness advantage themselves (especially via soil-soak where potting soil microbes might be producing antibiotics), it's best to use an "antibiotic swap" experimental design. For this, you have two pairs of strains: Strain1-GmR vs. Strain2-KmR  AND Strain1-KmR vs. Strain2-GmR. This will let you ensure that the antibiotic marker is not causing any competitive phenotypes you detect. 

* **Timing (tomato assays)**:
Option 1: **Synchronized disease stage**. At symptom onset (DI=1), tomato plants generally have 10^8-10^9 cfu/g stem. If you want to see which strain outcompetes the other, you might choose to sample all plants at DI=1.  This can be advantageous after a soil-soak competition because many asymptomatic plants will have bacterial populations below the limit of detection (~10^3 cfu/g stem). However, by only harvesting symptomatic plants, you might overlook something biologically interesting that happens before symptom onset. 

Option 2: **Specific time points**. This is the ideal option for cut-petiole infections. If you only have enough plants & time for one timepoint, 2 dpi (48 hpi if possible) is ideal.  If you have more plants & time, do a time-course at 0, 1, 2, 3 dpi. 
    * At 2 days post inoculation with 1000 cfu, Ralstonia is usually at 10^8-10^9 cfu/g stem. 

* **Sampling site**:
    * **Cut-Petiole**: Sample at the site of inoculation `'+0'`and a distal site (e.g. 2 cm below the site of inoculation `'-2'`).
        * After cut-petiole, the bacteria will first establish at the site of inoculation, then below the site of inoculation before establishing above the site of inoculation. 
        *This probably reflects connectivity of vascular architecture*
    * **Soil-Soak**: Sample at the cotyledon junction
## Preparing inoculum for petiole inoculation. 
(Soil soak inoculation is similar, but requires larger volumes)

*	Streak out strains on CPG + antibiotics.  Grow at 28C for 2 days (up to 7 days)
*	Overnight in CPG broth (+antibiotics if the strain needs to maintain a plasmid; no antibiotics if all genetic constructs are stably integrated into the genome). Shaking at 28C. 
    * Volume depends on your purpose.  3 ml culture is fine for most purposes.  Soil-soak inoculums require much more bacteria, so aim for 50-100 ml in shaking flasks. 
* Prep inoculum. Centrifuge cells. Remove supernatant. Wash once. 
* Adjust each strain to OD = 0.1 in 10 ml sterile H2O. Confirm the OD on spec and add more cells/water as needed to reach OD=0.1. 
* Mix the strains 1:1. Then dilute the mixture to your desired inoculation density (e.g. 1e3 cfu / 2 ul). This should be 10 ul of cell suspension + 990 ul H2O, but you should verify the math. 
* Dilution plate inocula on both antibiotic plates to confirm that the strains are in equal proportions. If you are calculating competitive indices, you need to know the initial ratio of strains to normalize the final numbers. 

Follow the [petiole](tomato_petiole_inoc.md) or [soil soak](tomato_ss_inoc.md) inoculation protocols and the [stem colonization assay](col_tomato_stem.md) protocol for quantifying population size of each strain. 

Note: you will have to dilution plate onto agar with each antibiotic. 

Tiffany has an example lab notebook entry (word doc plan, excel spreadsheet with data, and GraphPad Prism visualization of the data) for a tomato petiole inoculation at: LPlab > nb-LowePower, Tiff > PI_science > Plant experiments. The files are datestamped with 20210224