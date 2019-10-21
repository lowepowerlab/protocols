# Primer Blast

**Writing/editing credits:** Tiffany Lowe-Power

Good news -- Primer blast now lets you save your search parameters!  
Please append any useful parameter combinations at the bottom of this protocol with a brief description of its purpose (especially if you find how to search against new Ralstonia genomes)

## Parameters

### PCR Template
* **Enter accession, gi, or FASTA sequence**: Paste in a fasta sequence e.g. from benchling
* **Range**: I use this most often when designing gene complements. 
I will set a **Forward Primer To** and **Reverse Primer From** that encompasses the regions-of-interest (e.g. to complement a gene with its native promoter (*cis* elements))

### Primer parameters
* **Use my own forward/revese primer)**: Generally use one or neither of these parameters. 
Useful for precise gene deletions. (**forward**) if you want a Downstream-F primer that just-follows a stop codon but doesn't interrupt the downstream gene, or (**reverse**) for an Upstream-R primer that just precedes a start but doesn't remove promoter elements.
* **PCR product size**:
  * 50-200 bp for quantitative PCR primers (e.g. qRT-PCR / dd-PCR)
  * 800-1200 bp for homologous recombination regions

* **Primer melting temperatures**: Generally you want to keep primers within 3 degrees(**Max Tm difference**), but increasing this to 10 can help you problem-solve a "no primers found" error.
  * **Opt**: 
    * For quantitative primers, *don't change* from 60C. 
    * For PCR screening primers, try not to deviate from 60C. 
    More details about design of PCR screening primers in [colony pcr protocol](colony_pcr.md)
    * For clonining primers, I often iterate 59 - 63 C to diversify the results. 
  After all parameters are set, checkmark **Show results in new window** > `Get Primers`; change the Opt by 1 degree > `Get Primers`; etc. 
    Because each primerblast result takes a few minutes to load, running in parallel saves time.
  * **Min/Max**: Change as needed

### Primer Pair Specificity Checking Parameters
* **Database**: NCBI keeps changing how this works... but as of 2019, this works:

| Strain    | Database           | Organism     |
|----------:|:------------------|:-----|
|  GMI1000 | nr         | GMI1000 | 
|  PSI07   |nr   | PSI07 | 
| IBSBF1503| nr | 305 |

Note: Only a few of the genomes are hand-picked by NCBI to be assigned "taxonomy IDs". If you are designing primers in one of those strains,  you can search against Ralstonia solanacearum taxid:**305**. It will be slower (more genomes are queried), and you will have to be more careful interpreting results (only pay attention to `products on intended targets`.).

### Before clicking `Get Primers`:
* Check **Show results in new window**

### What to pay attention to in the results page:
* You will always have to select a genome before the BLAST continues.  
The page will say: *"Your PCR template is highly similar to the following sequence(s) from the search database. To increase the chance of finding specific primers, please review the list below and select all sequences (within the given sequence ranges) that are intended or allowed targets."*
Select the genome and click `submit`.

On the result page:
1. Observe the `Graphical view of primer pairs`. Make sure primer hits are in regions where you expected / wanted them to be.  Depending on how stringent your search inputs, PrimerBlast may only provide 10 very similar primers +/- a few nt. 
1. Focus first: `Primers on intended targets`.
    * Ideally, you should only hit your intended PCR amplicon. 
    * If all 10 primers have non-specific hits, investigate the hits from `Opt Tm` +/- 1-3C. 
    * If you can't avoid non-specific hits, make sure they are much larger than your target (and keep your 72C extension step of your PCR as short as possible) & have multiple mismatched between primer & off-target region. 
1. Look at the Self-complementarity scores.  lower = better. Stay at 4 or less if you can be choosy. 

## Useful Saved Searches

1. Search against **GMI1000**. PCR product sizes ideal for homologous recombination (e.g. gene knockouts). 
[link](https://www.ncbi.nlm.nih.gov/tools/primer-blast/index.cgi?LINK_LOC=bookmark&OVERLAP_5END=7&OVERLAP_3END=4&PRIMER_PRODUCT_MIN=800&PRIMER_PRODUCT_MAX=1200&PRIMER_NUM_RETURN=20&PRIMER_MIN_TM=57.0&PRIMER_OPT_TM=61.0&PRIMER_MAX_TM=66.0&PRIMER_MAX_DIFF_TM=3&PRIMER_ON_SPLICE_SITE=0&SEARCHMODE=0&SPLICE_SITE_OVERLAP_5END=7&SPLICE_SITE_OVERLAP_3END=4&SPAN_INTRON=off&MIN_INTRON_SIZE=1000&MAX_INTRON_SIZE=1000000&SEARCH_SPECIFIC_PRIMER=on&EXCLUDE_ENV=off&EXCLUDE_XM=off&TH_OLOGO_ALIGNMENT=off&TH_TEMPLATE_ALIGNMENT=off&ORGANISM=Ralstonia%20solanacearum%20GMI1000%20%28taxid%3A267608%29&PRIMER_SPECIFICITY_DATABASE=refseq_representative_genomes&TOTAL_PRIMER_SPECIFICITY_MISMATCH=1&PRIMER_3END_SPECIFICITY_MISMATCH=1&MISMATCH_REGION_LENGTH=5&TOTAL_MISMATCH_IGNORE=6&MAX_TARGET_SIZE=4000&ALLOW_TRANSCRIPT_VARIANTS=off&HITSIZE=50000&EVALUE=30000&WORD_SIZE=7&MAX_CANDIDATE_PRIMER=500&PRIMER_MIN_SIZE=15&PRIMER_OPT_SIZE=20&PRIMER_MAX_SIZE=25&PRIMER_MIN_GC=20.0&PRIMER_MAX_GC=80.0&GC_CLAMP=0&NUM_TARGETS_WITH_PRIMERS=1000&NUM_TARGETS=20&MAX_TARGET_PER_TEMPLATE=100&POLYX=5&SELF_ANY=8.00&SELF_END=3.00&PRIMER_MAX_END_STABILITY=9&PRIMER_MAX_END_GC=5&PRIMER_MAX_TEMPLATE_MISPRIMING_TH=40.00&PRIMER_PAIR_MAX_TEMPLATE_MISPRIMING_TH=70.00&PRIMER_MAX_SELF_ANY_TH=45.0&PRIMER_MAX_SELF_END_TH=35.0&PRIMER_PAIR_MAX_COMPL_ANY_TH=45.0&PRIMER_PAIR_MAX_COMPL_END_TH=35.0&PRIMER_MAX_HAIRPIN_TH=24.0&PRIMER_MAX_TEMPLATE_MISPRIMING=12.00&PRIMER_PAIR_MAX_TEMPLATE_MISPRIMING=24.00&PRIMER_PAIR_MAX_COMPL_ANY=8.00&PRIMER_PAIR_MAX_COMPL_END=3.00&PRIMER_MISPRIMING_LIBRARY=AUTO&NO_SNP=off&LOW_COMPLEXITY_FILTER=on&MONO_CATIONS=50.0&DIVA_CATIONS=1.5&CON_ANEAL_OLIGO=50.0&CON_DNTPS=0.6&SALT_FORMULAR=1&TM_METHOD=1&PRIMER_INTERNAL_OLIGO_MIN_SIZE=18&PRIMER_INTERNAL_OLIGO_OPT_SIZE=20&PRIMER_INTERNAL_OLIGO_MAX_SIZE=27&PRIMER_INTERNAL_OLIGO_MIN_TM=57.0&PRIMER_INTERNAL_OLIGO_OPT_TM=60.0&PRIMER_INTERNAL_OLIGO_MAX_TM=63.0&PRIMER_INTERNAL_OLIGO_MAX_GC=80.0&PRIMER_INTERNAL_OLIGO_OPT_GC_PERCENT=50&PRIMER_INTERNAL_OLIGO_MIN_GC=20.0&PICK_HYB_PROBE=off&NEWWIN=off&NEWWIN=off&SHOW_SVIEWER=true)

### Avoiding Bad primers:
The following examples require you to copy the sequence from [this benchling document](https://benchling.com/s/seq-LdA7kp7esUiuZhGqPGeJ) into the PCR Template sequence.

**Problem 1** [Link](https://www.ncbi.nlm.nih.gov/tools/primer-blast/index.cgi?LINK_LOC=bookmark&PRIMER5_START=3072&PRIMER5_END=3122&OVERLAP_5END=7&OVERLAP_3END=4&PRIMER_PRODUCT_MIN=800&PRIMER_PRODUCT_MAX=1200&PRIMER_NUM_RETURN=20&PRIMER_MIN_TM=57.0&PRIMER_OPT_TM=61&PRIMER_MAX_TM=64.0&PRIMER_MAX_DIFF_TM=3&PRIMER_ON_SPLICE_SITE=0&SEARCHMODE=0&SPLICE_SITE_OVERLAP_5END=7&SPLICE_SITE_OVERLAP_3END=4&SPAN_INTRON=off&MIN_INTRON_SIZE=1000&MAX_INTRON_SIZE=1000000&SEARCH_SPECIFIC_PRIMER=on&EXCLUDE_ENV=off&EXCLUDE_XM=off&TH_OLOGO_ALIGNMENT=off&TH_TEMPLATE_ALIGNMENT=off&ORGANISM=Ralstonia%20solanacearum%20GMI1000%20%28taxid%3A267608%29&PRIMER_SPECIFICITY_DATABASE=refseq_representative_genomes&TOTAL_PRIMER_SPECIFICITY_MISMATCH=1&PRIMER_3END_SPECIFICITY_MISMATCH=1&MISMATCH_REGION_LENGTH=5&TOTAL_MISMATCH_IGNORE=6&MAX_TARGET_SIZE=4000&ALLOW_TRANSCRIPT_VARIANTS=off&HITSIZE=50000&EVALUE=30000&WORD_SIZE=7&MAX_CANDIDATE_PRIMER=500&PRIMER_MIN_SIZE=15&PRIMER_OPT_SIZE=20&PRIMER_MAX_SIZE=25&PRIMER_MIN_GC=20.0&PRIMER_MAX_GC=80.0&GC_CLAMP=0&NUM_TARGETS_WITH_PRIMERS=1000&NUM_TARGETS=20&MAX_TARGET_PER_TEMPLATE=100&POLYX=5&SELF_ANY=8.00&SELF_END=3.00&PRIMER_MAX_END_STABILITY=9&PRIMER_MAX_END_GC=5&PRIMER_MAX_TEMPLATE_MISPRIMING_TH=40.00&PRIMER_PAIR_MAX_TEMPLATE_MISPRIMING_TH=70.00&PRIMER_MAX_SELF_ANY_TH=45.0&PRIMER_MAX_SELF_END_TH=35.0&PRIMER_PAIR_MAX_COMPL_ANY_TH=45.0&PRIMER_PAIR_MAX_COMPL_END_TH=35.0&PRIMER_MAX_HAIRPIN_TH=24.0&PRIMER_MAX_TEMPLATE_MISPRIMING=12.00&PRIMER_PAIR_MAX_TEMPLATE_MISPRIMING=24.00&PRIMER_PAIR_MAX_COMPL_ANY=8.00&PRIMER_PAIR_MAX_COMPL_END=3.00&PRIMER_MISPRIMING_LIBRARY=AUTO&NO_SNP=off&LOW_COMPLEXITY_FILTER=on&MONO_CATIONS=50.0&DIVA_CATIONS=1.5&CON_ANEAL_OLIGO=50.0&CON_DNTPS=0.6&SALT_FORMULAR=1&TM_METHOD=1&PRIMER_INTERNAL_OLIGO_MIN_SIZE=18&PRIMER_INTERNAL_OLIGO_OPT_SIZE=20&PRIMER_INTERNAL_OLIGO_MAX_SIZE=27&PRIMER_INTERNAL_OLIGO_MIN_TM=57.0&PRIMER_INTERNAL_OLIGO_OPT_TM=60.0&PRIMER_INTERNAL_OLIGO_MAX_TM=63.0&PRIMER_INTERNAL_OLIGO_MAX_GC=80.0&PRIMER_INTERNAL_OLIGO_OPT_GC_PERCENT=50&PRIMER_INTERNAL_OLIGO_MIN_GC=20.0&PICK_HYB_PROBE=off&NEWWIN=on&NEWWIN=on&SHOW_SVIEWER=true): 
There are only non-specific primers available. 
Sometimes it's still work gambling to see if you can use these primers. 
PCR is more likely to be successful if the non-specific products are substantially longer than the target-of-interest. 
You might be able to optimize your extension time to benefit the target-of-interest. 
    * **Avoid at all costs**: primers that have non-specific products that will not separate on a gel.

**Problem 2** [Link](https://www.ncbi.nlm.nih.gov/tools/primer-blast/index.cgi?LINK_LOC=bookmark&PRIMER5_START=3072&PRIMER5_END=3122&OVERLAP_5END=7&OVERLAP_3END=4&PRIMER_PRODUCT_MIN=800&PRIMER_PRODUCT_MAX=1200&PRIMER_NUM_RETURN=20&PRIMER_MIN_TM=57.0&PRIMER_OPT_TM=60&PRIMER_MAX_TM=66&PRIMER_MAX_DIFF_TM=3&PRIMER_ON_SPLICE_SITE=0&SEARCHMODE=0&SPLICE_SITE_OVERLAP_5END=7&SPLICE_SITE_OVERLAP_3END=4&SPAN_INTRON=off&MIN_INTRON_SIZE=1000&MAX_INTRON_SIZE=1000000&SEARCH_SPECIFIC_PRIMER=on&EXCLUDE_ENV=off&EXCLUDE_XM=off&TH_OLOGO_ALIGNMENT=off&TH_TEMPLATE_ALIGNMENT=off&ORGANISM=Ralstonia%20solanacearum%20GMI1000%20%28taxid%3A267608%29&PRIMER_SPECIFICITY_DATABASE=refseq_representative_genomes&TOTAL_PRIMER_SPECIFICITY_MISMATCH=1&PRIMER_3END_SPECIFICITY_MISMATCH=1&MISMATCH_REGION_LENGTH=5&TOTAL_MISMATCH_IGNORE=6&MAX_TARGET_SIZE=4000&ALLOW_TRANSCRIPT_VARIANTS=off&HITSIZE=50000&EVALUE=30000&WORD_SIZE=7&MAX_CANDIDATE_PRIMER=500&PRIMER_MIN_SIZE=15&PRIMER_OPT_SIZE=20&PRIMER_MAX_SIZE=25&PRIMER_MIN_GC=20.0&PRIMER_MAX_GC=80.0&GC_CLAMP=0&NUM_TARGETS_WITH_PRIMERS=1000&NUM_TARGETS=20&MAX_TARGET_PER_TEMPLATE=100&POLYX=5&SELF_ANY=8.00&SELF_END=3.00&PRIMER_MAX_END_STABILITY=9&PRIMER_MAX_END_GC=5&PRIMER_MAX_TEMPLATE_MISPRIMING_TH=40.00&PRIMER_PAIR_MAX_TEMPLATE_MISPRIMING_TH=70.00&PRIMER_MAX_SELF_ANY_TH=45.0&PRIMER_MAX_SELF_END_TH=35.0&PRIMER_PAIR_MAX_COMPL_ANY_TH=45.0&PRIMER_PAIR_MAX_COMPL_END_TH=35.0&PRIMER_MAX_HAIRPIN_TH=24.0&PRIMER_MAX_TEMPLATE_MISPRIMING=12.00&PRIMER_PAIR_MAX_TEMPLATE_MISPRIMING=24.00&PRIMER_PAIR_MAX_COMPL_ANY=8.00&PRIMER_PAIR_MAX_COMPL_END=3.00&PRIMER_MISPRIMING_LIBRARY=AUTO&NO_SNP=off&LOW_COMPLEXITY_FILTER=on&MONO_CATIONS=50.0&DIVA_CATIONS=1.5&CON_ANEAL_OLIGO=50.0&CON_DNTPS=0.6&SALT_FORMULAR=1&TM_METHOD=1&PRIMER_INTERNAL_OLIGO_MIN_SIZE=18&PRIMER_INTERNAL_OLIGO_OPT_SIZE=20&PRIMER_INTERNAL_OLIGO_MAX_SIZE=27&PRIMER_INTERNAL_OLIGO_MIN_TM=57.0&PRIMER_INTERNAL_OLIGO_OPT_TM=60.0&PRIMER_INTERNAL_OLIGO_MAX_TM=63.0&PRIMER_INTERNAL_OLIGO_MAX_GC=80.0&PRIMER_INTERNAL_OLIGO_OPT_GC_PERCENT=50&PRIMER_INTERNAL_OLIGO_MIN_GC=20.0&PICK_HYB_PROBE=off&NEWWIN=on&NEWWIN=on&SHOW_SVIEWER=true): 
Because of limited choices for primer placement and **Opt** primer temp, only primers with large Tm differences are output. 
Solution: iterate with different **Opt**, **Max**, or **Min** temps.
