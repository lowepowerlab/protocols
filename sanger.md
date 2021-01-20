# Sanger Sequencing Guide
This tells the SOP for Sanger Sequencing at UC Davis.

Generally, sequence 2-4 clones of every vector you intend to use & save down the E. coli in glycerol stocks.

Ideally sequence only after you have done colony PCR to confirm the vectors have an **appropriately sized** insert.

## Submitting sanger sequencing runs
There are two options. We prefer Eurofins due to the quality and cost. However, we need to have at least 9 samples in order to get the free shipping. 

If you just have a few reactions, you should use the UCD college of Biological Sciences DNA Sequencing facility: http://dnaseq.ucdavis.edu. 

### Prepare your sample (Eurofins)
This is general steps because Eurofins could update their process.  So look at our Eurofin's Sanger instructions.  https://eurofinsgenomics.com/en/products/dna-sequencing/seq-sample-submission-guidelines/ 

**Our Eurofins login information is in the "Ordering" google sheet within our lab shared Google Drive**

* Log your samples into the Eurofins submission site. 
* Apply the Eurofins barcodes to each tube.  (These are free. If we run low, order more from Eurofins)
* Add appropriate volume of plasmid to the tube. If you are using the common sequencing primers, you can have Eurofins add their own.  If using specific primers, follow Eurofin's instructions. 

* Put all tubes inside a zip lock bag. Put inside a small box with the Eurofins paperwork.  Secure tubes with packing material or tape the ziplock into the box so it doesn't rattle around (tubes could open). *Note: when possible, reuse ziploc bags / small boxes that we receive materials in.*

* Bring package to Hutchison Mailroom (Rm 361) before 8:30 AM to ensure UPS picks up. 
  * Outgoing packages are placed inside the room on floor in the area immediately to the right of the door - big sign on wall says "FedEx and UPS Pick Up"Bring the box to the UPS pick-up location in the Mail room on the 3rd floor. You can put the package in the mailroom overnight.  Plasmid DNA should be stable at room temperature for a while. 

* Eurofins will email you a link to your data within 1-2 days. 

* After you get the sequences, check the quality.  We are allowed to request sample re-runs for 10% of an order for free.  If you have < 500 bp of usable sequence, request a re-run on up to 10% of your samples. Forward your order information to GenomicsSupport@eurofins.com

### Sequencing with the Sanger Sequencing service on campus

(This might be incomplete)

* Follow guidelines on Website: http://dnaseq.ucdavis.edu/SampleSubmission.cfm. Brief things:

1. Primers (4 ul / sequencing run; 3 uM concentration*) and template DNA (6 ul / seq run; [concentration depends on size](http://dnaseq.ucdavis.edu/DNAPrep-Concentration.html) ) must be in 0.5 ml tubes with clear labels.
    * *Dilute the 10 uM working stocks of primers. e.g. 9 ul of 10 uM stock + 21 ul H2O = 30 ul. 

* Submit an order: http://dnaseq.ucdavis.edu/orders/. You'll need an account, a 

* Place in a ziplock bag & label with your name & the order number (generated when you submit)

* Drop off reaction in **0280 Storer Hall** (basement in the building connected to Hutchison)

## Submitting sanger sequencing runs externally
Sequence with Eurofins Genomics: https://eurofinsgenomics.com/en/home/

### Prepare your sample:


### Drop off your sample:




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
  * Gibson assembly can create Indels at junctions of fragments. Inspect those carefully if it's important. 
  * Look for SNPs (small red areas in grey area on bottom bar).
    * Inspect raw trace. If it is an N, make your own judgement call. Rename bases with *lowercase* bases if you think the .ab1 basecall was too stringent.
* Decide whether you have the "correct clone" (make an overnight & save it in -80) or whether you need to sequence additional clones.

    
