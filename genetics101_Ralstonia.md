## Genetic engineering of Ralstonia

**Writing/editing credits:** Tiffany Lowe-Power

This is a short guide on the common plasmids that we use. If you don't understand the jargon, try to teach it yourself and then check your knowledge with an expert. I highly drawing out your plasmid design on a white board and checking it with an expert. 

### pUFR80
This plasmid is used for creating clean deletion mutations. Key elements of this plasmid include:
* Suicide vector in Ralstonia. The oriR of this plasmid cannot replicate in Ralstonia.[xxx check this: This plasmid has an xxxx oriR, which is *E. coli* specific.]
* a lacZ multicloning site that enables **blue/white screening** (very helpful!). 
* a **negative selective marker (KanR)**  where antibiotic selection drives a vector to integrate into the genome next to the gene-of-interest followed by a 
* a **positive selection marker (sacB)** where sucrose sensitivity (conferred by SacB levanosucrase expressed from the vector backbone) 

**Downsides of pUFR80:** At 6.8 kb, the empty plasmid is fairly large. If you try to clone large things into it, most cloning efficiencies start to drop when the target plasmid approaches or exceeds 10 kb.

What sort of DNA inserts should you clone into pUFR80?
* Yes: Upstream and downstream regions (~800-1000 bp) of a gene to be deleted. 
* No: Pretty much anything else, including a construct to make a marked mutation. 

What should I consider before transforming Ralstonia with my pUFR80 construct?
* Do NOT linearize the plasmid backbone. Circular plasmid is key to the two-step selection. 

### pST-Blue
This plasmid is used for creating marked deletion mutations via allelic exchange. Key elements of this plasmid include:
* Suicide vector in Ralstonia. The oriR of this plasmid cannot replicate in Ralstonia.[xxx check this: This plasmid has an xxxx oriR, which is *E. coli* specific.]
* a lacZ multicloning site that enables **blue/white screening** (very helpful!). 
* small, high copy number plasmid. 
* Kan and Amp resistance in the backbone. Recommended to just use Kan to maintain the plasmid in E. coli. 

What should I consider before transforming Ralstonia with my pUFR80 construct?
* DO linearize the plasmid *backbone*. Linear plasmid increases the success of the double homologous recombination event that will yield a KO. 

* a **positive selection marker (sacB)** where sucrose sensitivity (conferred by SacB levanosucrase expressed from the vector backbone) 

What sort of DNA inserts should you clone into pUFR80?
* Yes: Upstream and downstream regions (~800-1000 bp) of a gene to be deleted. 
* No: constructs to replace a gene with Kan resistance. Since KanR is in the backbone, you should use a different plasmid to make a KanR mutation. 

### pMiniTn7 plasmids
These plasmids are used for inserting genes-of-interest into a selectively neutral location on the chromosome. 
[Read the paper on MiniTn7. Choi et al. 2006](https://www.nature.com/articles/nprot.2006.24). Chromosomal insertion has advantages -- after the initial selection and genetic confirmation, the insertion is stable, so antibiotics are not necessary to maintain the construct. There can be disadvantages: 

* Suicide vector in Ralstonia (and lots of other bacteria). The oriR of this plasmid cannot replicate in Ralstonia. These plasmids usually have a pUC origin, a high copy # origin that works in E. coli and related enterobacteriaceae. 
* a MiniTn7 that can insert next to the glmS gene if and only if you transform with a **helper plasmid** that expresses the tnsABCD transposase. The transposase genes are located in the parental Tn7, but they have been deleted from MiniTn7 so that the construct cannot continue to act as a jumping gene after it inserts. 
* Within the MiniTn7, we have several variants that have different resistance markers (Gent, Kan, etc.). We also have variants that express fluorescent proteins (e.g. GFP) There are lots of MiniTn7 variants in the literature that might be interesting. 

What sort of things is pMiniTn7 useful for
* Yes: 
    * Genetic complementation of a deletion. Note: You probably will need to use the native promoter. Identifying native promoters is a guess-and-check operation. Talk to folks in the lab for advice.  
    * Marking a strain with an antibiotic resistance cassette. 
    * Expressing a reporter gene (GFP, lux, etc.)
    * Heterologous expression of any gene.
* No: Any sort of construct to delete a gene.  


### pBBR1 origins make Ralstonia sick
This is a broad-host range replicative plasmid family. It will replicate in Ralstonia (meaning it is NOT a suicide plasmid). Unfortunately it also often yields Ralstonia colonies that look sickly. Tiffany has tried multiple versions of pBBR1-origin plasmids. pUFJ10 is a common pBBR1 origin plasmid that has been used in some Ralstonia strains successfully, but I don't recommend it. 
