## General Protocol for RB-TnSeq Experiments

**Written/Edited by**: Tiffany Lowe-Power, 

### Revive library aliquot

Library aliquots are stored in -80 C freezer as 1 ml of ~OD=0.800 culture (in 20% glycerol). 
This corresponds to ~4e8 to 8e8 cells, approx 500-1000x library size.

1. Thaw aliquot on wet ice. (~30 min).

2. Transfer to 100 ml CPG media containing 12.5 mg / ml Kan. 
   * Use an approach to temper the temperature change from 4 C to RT: Add some RT media to the 4C tube, transfer some cells to the flask.  Add more RT media to 4C tube, until all cells are transferred
   *  *Note*: This is 1/4th the normal Kan concentration.
   Wildtype GMI1000 is inhibited by as little as 2.5 mg / ml Kan, so this will still be selective. 
   But it might be 'gentler' on any mutants with increased Kan sensitivity.
1. Incubated at 28C with shaking overnight.
    * *XXX to update -- amount of time this takes on new shaker.  In Lindow lab, a timing of overnight starting at 4pm resulted in culture being ready at 9am-11am.*

### Harvest cells, adjust inoculum, save time 0, dilution plate

1. When cultures reach OD of 0.4 - 0.7, harvest cells.
Centrifuge 10 min 5k *xg* RT. 
1. Remove supernatant and resuspend cells. Measure OD. Adjust OD. 
    * Volume of resuspension depends on experimental design. 
    For in vitro experiments, resuspending in a few ml makes sense. 
    For petiole inoculation experiments, keep cells concentrated and measure OD of a 1:100 to 1:1000 dilution. 
    To inoculate plants with 1e8 cfu / plant, cell density will be OD = 100, so very very concentrated. 
    * Target OD will depend on experiment. Theoretically or empirically determine your target OD keeping in mind (1) Magnitude of a population bottleneck and (2) Trying to intro # of cells as >100x size of libraries (~2e5 individuals)
1. **Crucial**: Save duplicate time 0 (1e8-2e9 cfu; pelleted) in 1.5 ml tubes. 
Store in -20C.
1. *Highly recommended*: Dilution plate your inoculum to estimate 'initial population size'. If your experimental design allows you to estimate initial & final population size, you can normalize fitness values by # of population doublings in experiment.

### Perform selection experiment.

1. Add library to condition.
1. Allow library to grow in condition (ideally 5+ cell doublings; empirically determine appropriate timing with wildtype bacteria before using a library aliquot; see if you can estimate bottlenecks with wildtype as well)
1. Harvest bacteria after growth. 
    * *Highly recommended*: Dilution plate to estimate 'final population size' to later normalize fitness values by # doublings. 
1. Concentrate bacteria by a combination of selective filtering (>6 um filters to remove large debris; 0.22 um filters to collect bacteria on filter) or centrifugation. 
1. Save sample at -20 until DNA extraction.

### Extract DNA

1. Choose an appropriate DNA extraction kit.  
    * Kits like MoBio/Qiagen PowerSoil Powerlyzer kit are recommended for ~environmental samples (soil, maybe plant tissue) where humics/phenolics may be contaminating the DNA. These have similar charge to DNA, so co-purify with DNA in 'simple' kits, and they are potent PCR/enzyme inhibitors. 
    * For cleaner samples, use a cheaper DNA extraction kit like Qiagen Blood & Tissue. 
1. DNA extraction kits can impose bias (bigger issue for microbiome studies, but might affect some of the mutants in the library?), so within an experiment, use the same kit for time 0 and experimental samples. 

Submit sample for BarSeq analysis.

**Protocol/Guides to write**:
1. BarSeq
1. Data analysis
