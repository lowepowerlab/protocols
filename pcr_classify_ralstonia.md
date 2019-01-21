## PCRs to detect & classify plant pathogenic *Ralstonia*
**Writing/editing credit**: Caitilyn Allen lab, Tiffany Lowe-Power

## 1. Universal plant pathogenic *Ralstonia* PCR (759/760)

Detects a region present in most *R. solanacearum, R. pseudosolanacearum, R. syzygii* strains (82/85 tested by Opina)

**Citation**: Opina et al. 1997. A Novel Method For Development Of Species And Strain-Specific DNA Probes And PCR Primers For Identifying Burkholderia solanacearum (Formerly Pseudomonas solanacearum). Asia Pacific Journal of Molecular Biology and Biotechnology Volume 5, No. I, April, 1997 pp. l9-30.)

| Primer Name |  Sequence (5' to 3')             | 
|:-----------:|:---------------------------------|
|    759      | GTC GCC GTC AAC TCA CTT TCC      |
|    760      | GTC GCC GTC AGC AAT GCG GAA TCG  | 
**Product Size**: 281 bp

#### PCR conditions

* Controls: 
    1. No template control
    2. Positive control (e.g. gDNA from GMI1000)
* Calculate OneTaq or similar mastermix with [pcr_workbook](workbooks/pcr_workbook.xlsx)
* Thermal cycler conditions: Run OneTaq program with **58C anneal** & **30 s extension** time
* Resolve on **2%** agarose gel

## 2. Phylotype PCR (Multiplex)
**If reaction is positive, notify Tiffany Lowe-Power immediately.**

**Citation**: Fegan, M, and P. Prior 2005. How complex is the R. solanacearum species complex? In: Bacterial Wilt: The Disease and the Ralstonia solanacearum species complex (C. Allen, P. Prior, and A.C. Hayward, editors). APS Press, St Paul.

| Primer Name |  Sequence (5' to 3')    | Phylo specificity | Band size (bp)* |
|:-----------:|:------------------------|:-----------------:|:---------| 
| Nmult21:1F  | CGTTGATGAGGCGCGCAATTT   | I                 | 144      |
| Nmult21:2F  | AAGTTATGGACGGTGGAAGTC   | II                | 372      |
| ßNmult23:AF | ATTACSAGAGCAATCGAAAGATT | III               | 91       |
| Nmult22:InF | ATTGCCAAGACGAGAGAAGTA   | IV                | 213      |
| Nmult22:RR  | TCGCTTGACCCTATAACGAGTA  | all               | N/A      |


#### PCR conditions

* Controls: 
    1. No template control
    2. Positive control (ideally 1 strain from each phylotype, but at a minimum do a gDNA from a known isolate)
* ***XXX Someone needs to add this to pcr_workbook*** Reactions were carried out in a total volume of 20 µl containing 1 x PCR buffer (supplied by the manufacturer of the polymerase) 1.5 mM MgCl2, 0.2 mM of each dNTP, 2U of Taq Polymerase 6 pmoles of the primers Nmult:21:1F, Nmult:21:2F, Nmult:22:InF, 18 pmoles of the primer Nmult:23:AF and 4 pmoles of the primers 759 and 760 (1). Reactions were heated to 96oC for 5 min and then cycled through 30 cycles of 94oC for 15s, 59oC for 30s and 72oC for 30s, followed by a final extension period of 10 min at 72oC. 

* Thermal cycler conditions: Run OneTaq program with **59C anneal** & **30 s** extension time
* Resolve on **2%** agarose gel

Expected results:
![gel image of phylotype pcr results](images/phylotype_pcr_result.png)

## 3. Detection of Race 3 Biovar 2 strains
**If reaction is positive, notify Tiffany Lowe-Power immediately.**

**Citation**: Opina et al. 1997. A Novel Method For Development Of Species And Strain-Specific DNA Probes And PCR Primers For Identifying Burkholderia solanacearum (Formerly Pseudomonas solanacearum). Asia Pacific Journal of Molecular Biology and Biotechnology Volume 5, No. I, April, 1997 pp. l9-30.)

| Primer Name |  Sequence (5' to 3')             | 
|:-----------:|:---------------------------------|
|    630      | ATA CAG AAT TCG ACC GGC ACG      |
|    631      | ATT CAC ATG CAA TTC GCC TAC      | 
**Product Size**: 307 bp

#### PCR conditions

* Controls: 
    1. No template control
    2. Positive control (We do not have access to live Race 3 strains, but Caitilyn Allen's lab generously purified DNA from UW551 for us)
* Calculate OneTaq or similar mastermix with [pcr_workbook](workbooks/pcr_workbook.xlsx)
* Thermal cycler conditions: Run OneTaq program with **60C anneal** & **30 s** extension time
* Resolve on **2%** agarose gel
* **If reaction is positive, notify Tiffany Lowe-Power immediately.**

