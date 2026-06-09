# Chaotropic salt lysis and spin-column DNA purification
Protocol drafted by Gina Shin 

## Reagent Recipes

### Lysis buffer
*The lysis buffer is composed of a high concentration of guandidine hydrochloride, a chaotropic salt, as well as Tween-20, a detergent. Additionally, Tris-HCl buffer is added to the solution to help keep it at a neutral-to-slightly-alkaline pH.*

**To prepare 50mL of lysis buffer:**
1. **Add 19.1 grams of guanidine hydrochloride to a conical tube or bottle.** *This will be a large volume of salt and may fill most if not all of the container if you're using a container with a maximum volume around 50 mL.*
2. **Add 35 mL of MilliQ filtered water to the guanidine hydrochloride to dissolve it.** *With this volume, the concentration will be near 6 M. At room temperature, 6 M is roughly the maximum solubility. Additionally, the reaction is endothermic, so you will need to warm the solution to get it to fully dissolve.*
3. Once the guanidine hydrochloride is dissolved, **add 500 microliters of 1 M Tris-HCl at 7.5 pH.** *Lysis should not require highly alkaline conditions, however detergent effectiveness and guanidine hydrochloride solubility can decrease in highly acidic conditions. If you are getting poor lysis, double check that the pH of the lysis buffer and ensure it is near a neutral pH.*
4. After adding the Tris-HCl, **bring the volume of the solution up to 50 mL with MilliQ filtered water.** 
5. Once the solution is brought up to 50 mL, **add 250 microliters of Tween-20 solution and mix.** *Tween-20 is added last just to limit any issues arising from the detergent causing a lot of bubble formation, making volume measurements difficult.*

*This should generally be shelf-stable at room temperature. If precipitates form, it is likely guanidinium salts and you can gently warm the solution to re-dissolve any precipitates.*
**Do not let this solution get on your skin and read the SDS for the chemicals in this lysis buffer before using or preparing the solution.**

### Acetate buffer

*Acetate buffer is used as a component of the DNA binding buffer. This helps keep the pH low, which put simply, reduces negative charge interactions between the silica in spin columns and the phosphate backbone of DNA.*

**To prepare a 50 mL acetate buffer:**
1. **Add 0.25 grams of sodium acetate (anhydrous) to conical tube or bottle.**
2. **Add 40 mL of MilliQ filtered water to dissolve the sodium acetate.**
3. **Add 0.1 mL of glacial acetic acid to the solution.**
4. **Measure the pH and adjust it to sit within a range of 4.9-5.1.**
5. Once the pH is adjusted, **bring the total volume to 50 mL.**

This will produce roughly a 100 mM acetate/acetic acid solution. 
*While it is not necessary to filter-sterilize this solution, **filter-sterilization can help improve the shelf life** by reducing the chance of contaminants growing that use the acetate as a food source.*

### DNA Binding Buffer

*The alcohol and acidity of this solution will precipitate the DNA in your lysate and help it bind to silica.*

**To prepare 10 mL of DNA Binding Buffer:**
1.	**In a 15 mL conical tube, add 2 mL of the acetate buffer.**
2.	**Bring the volume up to 10 mL using reagent ethanol.** *The bulk reagent ethanol we buy is ok; it is not necessary to use molecular grade ethanol.*

Do not prepare large amounts of this, it is quick to prepare and contains alcohol which can evaporate over time.

### Wash solution 1

*Wash solution 1 contains guanidine hydrochloride and ethanol. This wash should help remove salt on the column, while also removing residual proteins off the column. The water and ethanol can help remove salt. The guanidine hydrocholoride can help remove residual proteins. Because this buffer still contains guanidine hydrocholoride, it will not fully remove salt off of the column, which is why an additional wash will be necessary.*

**To prepare 10 mL of wash solution 1:**
1.	**In a 15 mL conical tube, add 0.5 grams of guanidine hydrochloride.**
2.	**Add 7 mL of reagent alcohol to dissolve the guanidine hydrochloride.** This should take some time, but it should dissolve. *The bulk reagent ethanol we buy is ok; it is not necessary to use molecular grade ethanol.*
3.	Once the guanidine hydrochloride is dissolved, **bring the volume to 10 mL with MilliQ filtered water.**
   
Do not prepare large amounts of this, it is quick to prepare and contains alcohol which can evaporate over time.

### Wash Solution 2

*This wash solution will help remove any residual salt off of the column. It also contains a Tris-HCl buffer which will help shift our pH to prepare the DNA for elution. While the pH will begin to shift, the high ethanol concentration should keep the DNA bound to the silica.*

**To prepare 10 mL of wash solution 2:**
1.	**In a 15 mL conical tube, add 100 microliters of 1 M Tris-HCl, pH 7.5-8**
2.	**Add 7 mL of reagent ethanol.** *The bulk reagent ethanol we buy is ok; it is not necessary to use molecular grade ethanol.*
3.	**Bring the volume up to 10 mL with MilliQ filtered water.**

Do not prepare large amounts of this, it is quick to prepare and contains alcohol which can evaporate over time.

## Extraction & Purification Protocol

### Lysis and DNA Binding

*This protocol was designed to work with liquid overnight cultures. Hypothetically, it could work with a suspended colony, but I’m not sure if it will require additional wash steps because of the additional EPS.*

**Starting with an overnight culture:**
1.	**Pellet roughly 1-5x10<sup>8</sup> cfu.** This would be 1 mL of culture with an OD600 of 0.2 to 1. *Less is more in this case. This protocol does not include a proteinase K digestion step, so too many cells can clog your spin-column*
2.	**Discard the supernatant and resuspend your pellet in 200 microliters of lysis buffer.**
3.	**Incubate your suspension for 9 minutes at 70 °C. Invert your sample to mix every 3 minutes.**
4.	After incubation, **add 300 microliters of DNA binding buffer and mix vigorously** by pipetting or vortexing. *A precipitate may form, if so try to break it up by pipetting*
5.	**Transfer the entire solution, including any precipitate, to a spin-column that is placed in a collection tube.** *Any silica-based spin-column should work; this protocol was tested with UPrep columns.*
6.	**Centrifuge for 2 minutes at 10,000 rcf. Discard the flow-through.**

### Washing

*At this point, the DNA should be bound to the silica in the spin column. The next few steps are to purify the DNA on the column*

7.	**Add 400 microliters of wash solution 1. Let the wash buffer sit on the column for at least 1 minute, then centrifuge the spin column for 1 minute at 10,000 rcf. Discard the flow-through.**
8.	**Add 600 microliters of wash solution 2. Let the was buffer sit on the column for at least 1 minute, then centrifuge the spin column for 1 minutes 10,000 rcf. Discard the flow-through.** 
9.	Without adding any additional solutions, **centrifuge the spin column again for 2 minutes at 16,000 rcf.** *This step is meant to remove any residual alcohol from the column. Alcohol absorbs light at 230 nm and will interfere with quantification on a nanodrop. It can also inhibit PCR reactions*

### Elution

10.	 **Transfer your spin column to a 1.7 mL centrifuge tube.**
11.	 **Add your favorite elution solution to the column**; elution solutions can be water, tris-buffer, tris-EDTA buffer, etc… *DNA will release from the column at slightly alkaline conditions, so just make sure your water isn’t acidic. Warming your elution buffer can also increase your yield. For Ralstonia, if you started with 5x10<sup>8</sup> cfu, eluting with 100 microliters to 10 mM Tris buffer at pH 7.5, you will likely get a solution around 10 ng DNA/microliter.*
12.	 **Incubate your column for at least 1 minute, then centrifuge your column for 1 minute at 10,000 rcf.**

***Happy pipetting!***










# Phenol:Chloroform High-Molecular-Weight Genomic DNA Extraction from Bacterial Cultures of the *Ralstonia solanacearum* Species Complex

**Adapted from:** Nomenjanahary et al. 2025 (https://doi.org/10.1094/PHYTOFR-10-24-0110-A)

**Modified by:** Gina Shin (Lowe-Power Lab, UC Davis)

## Overview

This protocol describes the extraction of high-molecular-weight (HMW) genomic DNA from overnight cultures of members of the *Ralstonia solanacearum* species complex (RSSC). The procedure uses SDS-mediated cell lysis, Proteinase K digestion, phenol-chloroform purification, RNase treatment, and isopropanol precipitation to recover genomic DNA suitable for long-read sequencing applications.

## Reagents

| Reagent                                                                           | Supplier                 | Catalog Number |
| --------------------------------------------------------------------------------- | ------------------------ | -------------- |
| 1X TE Buffer (10 mM Tris-HCl, 1 mM EDTA, pH 8.0)                                  | In-house                 | In-house       |
| NaCl (5 M)                                                                        | In-house                 | In-house       |
| NaCl (0.5 M)                                                                      | In-house                 | In-house       |
| SDS (10%)                                                                         | In-house                 | In-house       |
| Proteinase K (20 mg/ml)                                                           | NEB                      | P8107S         |
| RNase A (20 mg/ml)                                                                | NEB                      | T3018L         |
| Phenol:Chloroform:Isoamyl alcohol (25:24:1, pH 8.0)                               | Thermo Fisher Scientific | 15593049       |
| Chloroform:Isoamyl alcohol (24:1)                                                 | Sigma-Aldrich            | C0549-1PT      |
| Isopropanol (molecular grade)                                                     | Sigma-Aldrich            | I9516          |
| 70% ethanol (prepared using molecular-grade ethanol and DNase-, RNase-free water) | In-house                 | In-house       |

**Note:** Reagents should be no older than six months.

## Before You Begin

### Purpose

Prepare reagents and equipment before beginning the extraction procedure.

### Preparation

* Chill isopropanol and 70% ethanol prior to use.
* Preheat water baths or heating blocks to 37°C, 55°C, and 65°C.
* Ensure phenol:chloroform:isoamyl alcohol is equilibrated to pH 8.0 or use pH 8.0 equilibrated reagents.
* Use freshly grown overnight bacterial cultures.

---

# Cell Harvesting and Washing

### Purpose

The NaCl wash removes residual growth medium, extracellular polysaccharides, and other contaminants that may interfere with cell lysis and downstream DNA purification.

### Procedure

1. Transfer 1.5 ml of overnight culture to a 2 ml microcentrifuge tube.
2. Centrifuge for 5 min at 5,000 × g.
3. Discard the supernatant.
4. Resuspend the cell pellet in 1 ml of 0.5 M NaCl and mix by pipetting using a 1000 µl pipette tip.
5. Centrifuge for 5 min at 5,000 × g.
6. Discard the supernatant.

---

# Cell Lysis and Protein Digestion

### Purpose

TE buffer stabilizes genomic DNA during extraction. Tris-HCl maintains pH, while EDTA chelates divalent cations required by many nucleases. SDS disrupts bacterial membranes and denatures proteins, releasing nucleic acids into solution. Proteinase K digests proteins, including nucleases that could degrade genomic DNA. Addition of concentrated NaCl promotes dissociation of protein-DNA complexes and facilitates removal of protein contaminants during organic extraction.

### Procedure

1. Resuspend the washed cell pellet in:

   * 567 µl 1X TE buffer
   * 30 µl 10% SDS
2. Add 3 µl Proteinase K (20 mg/ml).
3. Gently mix by pipetting using a 1000 µl pipette tip.
4. Incubate at 55°C for 2–3 h.
5. Add 100 µl 5 M NaCl.
6. Mix by pipetting using a 1000 µl pipette tip.
7. Incubate at 65°C for 10 min.

---

# Organic Extraction and RNA Removal

### Purpose

Phenol:chloroform:isoamyl alcohol separates proteins and other cellular contaminants from nucleic acids. Phenol denatures proteins, chloroform improves phase separation, and isoamyl alcohol reduces foaming. RNase A removes co-purifying RNA. A final chloroform extraction removes residual phenol, which can interfere with downstream applications and reduce DNA purity.

### Procedure

1. Add an equal volume (approximately 700 µl) of phenol:chloroform:isoamyl alcohol (25:24:1).
2. Mix by pipetting using a 1000 µl pipette tip.
3. Centrifuge for 20 min at 4°C at maximum speed.
4. Transfer the aqueous upper phase to a new 1.5 ml tube.
5. Add 10 µl RNase A (20 mg/ml).
6. Incubate for 30 min at 37°C.
7. Add an equal volume of phenol:chloroform:isoamyl alcohol (25:24:1).
8. Mix by pipetting using a 1000 µl pipette tip.
9. Centrifuge for 20 min at 4°C at maximum speed.
10. Transfer the aqueous upper phase to a new 1.5 ml tube.
11. Add an equal volume of chloroform:isoamyl alcohol (24:1).
12. Mix by pipetting using a 1000 µl pipette tip.
13. Centrifuge for 20 min at 4°C at maximum speed.
14. Transfer the aqueous upper phase to a new 1.5 ml tube.

---

# DNA Precipitation

### Purpose

Isopropanol reduces DNA solubility and promotes precipitation of high-molecular-weight genomic DNA. The presence of salt facilitates efficient DNA recovery. Overnight incubation at −20°C improves precipitation yield.

### Procedure

1. Add 0.6 volumes of ice-cold isopropanol.
2. Gently invert the closed tube to facilitate filamentous DNA precipitation.
3. Incubate at −20°C overnight.
4. Centrifuge for 20 min at 4°C at maximum speed.
5. Discard the supernatant.

---

# DNA Washing

### Purpose

Ethanol washes remove residual salts, phenol, and other contaminants while maintaining DNA precipitation. Two washes improve DNA purity for downstream sequencing applications.

### Procedure

1. Add 1 ml of ice-cold 70% ethanol.
2. Centrifuge for 20 min at 4°C at maximum speed.
3. Discard the supernatant.
4. Add 1 ml of ice-cold 70% ethanol.
5. Centrifuge for 20 min at 4°C at maximum speed.
6. Discard the supernatant.

---

# DNA Rehydration

### Purpose

Removal of residual ethanol improves downstream enzymatic reactions and sequencing performance. TE buffer protects DNA during storage and promotes recovery of high-molecular-weight DNA. Gentle warming facilitates complete DNA rehydration.

### Procedure

1. Briefly dry the DNA pellet by incubating the tube on a 70°C heating block for approximately 1 min.

   **Important:** Do not overdry the pellet. As soon as the pellet becomes transparent, remove the tube from the heating block.

2. Add 100 µl of 1X TE buffer (pH 8.0).

3. Incubate at 65°C for 30 min to rehydrate genomic DNA.

4. Pipette fewer than 10 times using a 200 µl pipette tip to gently dislodge and break apart the pellet.

---

# Quality Control

Assess DNA quantity and quality using:

* Qubit dsDNA assay
* Nanodrop spectrophotometry

  * A260/A280 ≈ 1.8–2.0
  * A260/A230 > 2.0
* Agarose gel electrophoresis

High-quality DNA should appear as a high-molecular-weight band with minimal smearing.

## Expected Outcome

This protocol yields high-molecular-weight genomic DNA suitable for long-read sequencing applications, including PacBio and Oxford Nanopore sequencing.

