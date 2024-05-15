## General Protocol for RB-TnSeq Experiments

**Written/Edited by**: Tiffany Lowe-Power, 

### Revive library aliquot

Library aliquots are stored in -80 C freezer as 1 ml of ~OD=0.800 culture (in 20% glycerol). 
This corresponds to ~4e8 to 8e8 cells, approx 500-1000x library size.

1. Thaw aliquot on wet ice. (~30 min).

2. Transfer to 100 ml CPG media containing 12.5 mg / ml* Kan (see note). 
   * Use an approach to temper the temperature change from 4 C to RT: Add some RT media to the 4C tube, transfer some cells to the flask.  Add more RT media to 4C tube, until all cells are transferred
   *  **Note*: This is 1/2 the normal Kan concentration.
   Wildtype GMI1000 is inhibited by as little as 2.5 mg / ml Kan, so this will still be selective. 
   But it might be 'gentler' on any mutants with increased Kan sensitivity.
3. Incubate at 28C with shaking overnight.
    * *XXX to update -- amount of time this takes on new shaker.  In Lindow lab, a timing of overnight starting at 4pm resulted in culture being ready at 9am-11am.*

### Harvest cells, adjust inoculum, save time 0, dilution plate

1. When cultures reach OD of 0.4 - 0.7, harvest cells.
Centrifuge 10 min 5k *xg* RT. 
2. Remove supernatant (wash 2x if residual rich media is likely to skew experimental results) and resuspend cells. Measure OD. Adjust OD. 
    * Volume of resuspension depends on experimental design. 
    For in vitro experiments, resuspending in a few ml makes sense. 
    For petiole inoculation experiments, keep cells concentrated and measure OD of a 1:100 to 1:1000 dilution. 
    To inoculate plants with 1e8 cfu / plant, cell density will be OD = 100, so very very concentrated. 
    * Target OD will depend on experiment. Theoretically or empirically determine your target OD keeping in mind (1) Magnitude of a population bottleneck and (2) Trying to intro # of cells as >100x size of libraries (~2e5 individuals)
3. **Crucial**: Save duplicate time 0 (1e8-2e9 cfu; pelleted) in 1.5 ml tubes and store in -20C.
Adam D. recommends recovering a single aliquot of the mutant library in a single flask. Then collecting 8 cell pellets for the Time 0. This culture will be used to set up all of your biological replicate experiments. You can do genomic preps and barseq of at least 4 of these Time 0 samples. It's better to collect 8 because Adam can have Time 0 samples on different genomic DNA/BarSeq plates if the samples end up getting spread across multiple plates. 
4. *Highly recommended*: Dilution plate your inoculum to estimate 'initial population size'. If your experimental design allows you to estimate initial & final population size, you can normalize fitness values by # of population doublings in experiment.

### Perform selection experiment.

1. Add library to condition.
2. Allow library to grow in condition (ideally 5+ cell doublings; empirically determine appropriate timing with wildtype bacteria before using a library aliquot; see if you can estimate bottlenecks with wildtype as well)
3. Harvest bacteria after growth. 
    * *Highly recommended*: Dilution plate to estimate 'final population size' to later normalize fitness values by # doublings. 
4. Concentrate bacteria by a combination of selective filtering (>6 um filters to remove large debris; 0.22 um filters to collect bacteria on filter) or centrifugation. 
5. Save sample at -20 until DNA extraction.

### Extract DNA

1. Choose an appropriate DNA extraction kit.  
    * Kits like MoBio/Qiagen PowerSoil Powerlyzer kit are recommended for ~environmental samples (soil, maybe plant tissue) where humics/phenolics may be contaminating the DNA. These have similar charge to DNA, so co-purify with DNA in 'simple' kits, and they are potent PCR/enzyme inhibitors. 
    * For cleaner samples, use a cheaper DNA extraction kit like Qiagen Blood & Tissue. 
2. DNA extraction kits can impose bias (bigger issue for microbiome studies, but might affect some of the mutants in the library?), so within an experiment, use the same kit for time 0 and experimental samples. 

Submit sample for BarSeq analysis.

**Protocol/Guides to write**:
1. BarSeq
2. Data analysis
