# Sanger Sequencing Guide
This tells the SOP for Sanger Sequencing at UC Davis.

Generally, sequence 2-4 clones of every vector you intend to use & save down.  
Ideally sequence only after you have done colony PCR to confirm the vectors have an appropriately sized insert.

## Submitting sanger sequencing runs
Things to figure out:
1. How labs in Hutch do sanger sequencing -- Genome center?
1. How the seq center prefers to receive tubes (strip tubes? 1.5 mls?). How much primer, how much Template
1. How to access the sanger files
1. SOP for naming the file... e.g. systematic plasmid & primer names?  Date stamp is usually applied by the seq center

## What to do after you've downloaded the sanger files
probably .ab1 traces

Save them into a logical folder (e.g. a "Sanger Results" folder in your Cloning folder)

### Benchling Approach
This approach allows you to overlay the sequence *and* raw trace with your DNA-of-interest

* Open your plasmid plan in Benchling (you made one right ಠ_ಠ)
* Click the **Alignments** tool on the right > `Create New Alignment` > `Choose Files` (Choose all ab1 files that map). > `Create Alignment`
* Inspect the Alignment for sanger seq quality
  * Does it match at all? Bottom of the screen will be a diagram showing grey=match and red =mismatch.
  * How was the sequencing quality (abunance of "Ns", which will print as red at the bottom & also raw traces--are there clear & equally spaced peaks)?  
    * If sequence is gibberish (entirerly or <200 bp usable sequence) email the seq center and request a *free rerun*.
* If sequencing quality is good... look for problems.  
  * Gibson assembly can create Indels at junctions of fragments.  Inspect those carefully if it's important.  
  * Look for SNPs (small red areas in grey area on bottom bar).
    * Inspect raw trace.  If it is an N, make your own judgement call.  Rename bases with *lowercase* bases if you think the .ab1 basecall was too stringent.
* Decide whether you have the "correct clone" (make an overnight & save it in -80) or whether you need to sequence additional clones.

    
