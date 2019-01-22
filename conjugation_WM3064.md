## Conjugation with *E. coli* WM3064 

### Strain WM3064

**Genotype**: *thrB1004 pro thi rpsL hsdS lacZΔM15 RP4-1360 Δ(araBAD)567 ΔdapA1341::[erm pir]*

**Purpose** Is auxotrophic for DAP (diaminopimelic acid - a lysine precursor). The auxotrophy enables removal of this strain from a bi-parental mating setup after conjugation. This strain can be used for conjugation experiments and replication of plasmids that require Pir protein.

Strain was derived from *E. coli* B2155 by William Metcalf at UIUC.

## Protocol

### Preparation:

* E. coli WM3064 carrying plasmid of interest e.g. pUFR80, pST-Blue, or pKMW3 derivatives
* Media:
    * LB + 300 uM DAP + antibiotic 
    * CPG + 300 uM DAP
    * CPG+DAP-Glc Modified CPG plates: (no glucose or TZC, + 300 uM DAP) *4 plates per transformation*
    * CPG +TZC + antibiotic plates
* Cut 80 mm nitrocellulose filters (0.45 um pore size) into 6ths and autoclave. 
Overlay filters on CPG+DAP-Glc plates. 
If doing multiple replicates of the same donor/recipient, you can add up to 4 filters/plate. 
Keep different strains on separate plates to avoid cross-contamination--sometimes liquid droplets bounce/spray. 

### Methods
1. **Day 0**: Streak *Ralstonia* strain on CPG plate. 
Incubate at 28C for 2 days
1. **Day 1**: *Optional* Streak out *E. coli* WM3064+plasmid onto LB+DAP+antibiotic plate. 
Incubate at 37C overnight.
1. **Day 2**: Inoculate a single colony of *Ralstonia* into 5 ml CPG broth.
Incubate overnight 28C with 180 rpm shaking.
    * *Optional* - Start overnight culture of *E. coli* WM3064+plasmid in 3 ml LB+DAP+antibiotic broth.
1. **Day 3**: Grow cells to mid-log before initiating transformation. 
    1. *E. coli*: Either subculture 500 ul of the overnight culture into 4.5 ml LB+DAP+antibiotic in XXX mm test tube or thaw 1 ml -80C aliquot on ice before subculturing it into 25 ml pre-warmed LB+DAP+antibiotic in 125 ml flask. 
    Grow at 37C with shaking until mid-log (OD 0.5-0.8). 
    1. *Ralstonia*: Dilute 2 ml of overnight culture into 25 ml pre-warmed CPG broth in 125 ml flask. 
    Incubate at 28C with shaking until E. coli is ready. 
    Record OD of *Ralstonia* isolate in notebook. 
1. Pellet cultures (8k *xg* for 5 min). 
Resuspend in 1 ml CPG+DAP. 
Transfer to 1.5 ml tube and pellet (>13k *xg* for 1 min). 
Repeat wash with additional 1 ml CPG+DAP.  
Resupend in 1 ml CPG+DAP.
1. Measure OD of 1:10 or 1:100 dilution of cell suspensions. 
Use [bacterial_density_workbook](workbooks/bacterial_density_workbook.xlsx) to adjust *Ralstonia* density to OD = 3 and *E. coli* density to OD = 1. 
1. Mix even volumes of *Ralstonia* and *E. coli* (creating a 3:1 ratio of recipient:donor strain). 
1. Plate 100 ul of the suspension on the center of a nitrocellulose filter on CPG+DAP-Glc plate. 
Allow spot to dry on filter (incubate without lid in Biosafety Cabinet or laminar flow hood to accelerate drying)
1. Incubate at 28 C for 2 - 4 h. 
1. Select transconjugants.
1. Transfer filter with conjugation spot to 2.0 ml tube with 1 ml CPG. 
1. Vortex 10-30 s to dislodge bacteria. 
1. Plate 100 ul of a dilution series: 10<sup>0</sup>, 10<sup>-1</sup>, 10<sup>-2</sup>, 10<sup>-3</sup>, and 10<sup>1</sup>(the remaining cells resuspended in 100 ul). 
1. Incubate plates at 28 C for 2 days (up to 4 days). 
As soon as colonies appear, restreak for purity. 
Follow up with [colony pcr](colony_pcr.md) to genotype.

*Note about transformation efficiency*: Transformation with pKMW3 derivative in 2018-11 yielded efficiencies (# transformants = # colonies on antibiotci plate / total # cells = # colonies on CPG plate) of 3.9x10<sup>-5</sup> to 8.6x10<sup>-3</sup>. 