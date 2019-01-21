## Gene deletion in *Ralstonia*

**Writing/editing credits:** Tiffany Lowe-Power

This protocol describes two strategies for gene deletion in *Ralstonia* spp. The **marked gene deletion** approach involves a negative selection approach where a an antibiotic resistance cassette is swapped into in the place of a gene-of-interest (via double homologous recombination AKA allelic exchange).  The **unmarked gene deletion** involves (1) a negative selection where antibiotic selection drives a vector to integrate into the genome next to the gene-of-interest followed by a (2) positive selection where sucrose sensitivity (conferred by *sacB* on the vector backbone) drives the vector to recombine out of the genome resulting in ~50% wildtype and 50% knockout genotype clones. 

<!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [What is a repository/repo?](#what-is-a-repositoryrepo)
- [Git vs Github](#git-vs-github)
- [Git and GitHub Setup and Basic Commands](#git-and-github-setup-and-basic-commands)
	- [GitHub signup](#github-signup)
	- [Play with GitHub](#play-with-github)
	- [Set Up a Text Editor on your computer](#set-up-a-text-editor-on-your-computer)
	- [Install Git on your computer](#install-git-on-your-computer)
	- [Play with Git](#play-with-git)
	- [Some notes about local Git repos:](#some-notes-about-local-git-repos)
- [Forking and cloning the `protocols` repo](#forking-and-cloning-the-protocols-repo)
	- [Fork the repo to your GitHub account](#fork-the-repo-to-your-github-account)
	- [Upstream vs Remote vs Local versions of the repo](#upstream-vs-remote-vs-local-versions-of-the-repo)
	- [Modify a lab protocol](#modify-a-lab-protocol)
	- [Short commit message](#short-commit-message)
	- [Pull Request: Now suggest this change to the lab](#pull-request-now-suggest-this-change-to-the-lab)
- [Dealing with the situation where your Remote repo (`mandel01/protocols`) is different from the lab Upstream repo (`mjmlab/protocols`)](#dealing-with-the-situation-where-your-remote-repo-mandel01protocols-is-different-from-the-lab-upstream-repo-mjmlabprotocols)

<!-- /TOC -->



### Marked gene deletion 

### Unmarked gene deletion (sacB)

#### Resources:
* [pUFR80 vector map with sequence](https://benchling.com/s/SGEEU7/edit) 
* [Primer Design with PrimerBlast](primerblast.md)
* [Plasmid Assembly with Gibson Assembly](gibson_assembly.md)
* [Proof Checking your assembled plasmid](plasmid_proofing.md)

#### Clone the knockout vector:
Clone approximately 0.9-1.2 kb upstream DNA and 0.9-1.2 kb downstream DNA adjacent to each other. Aim for similar sized upstream and downstream fragments so that crossovers on either flanking side are equally likely. Try to have the up/downstream regions immediately up/downstream from the start and stop codons, respectively. Take care to avoid disrupting neighboring or overlapping genes.

Suggested method: Gibson Assembly cloning in pUFR80. The following protocol assumes a vector containing kanamycin resistance was used, the CPG-Kan concentration was 25 μg/ml unless otherwise stated, and all solid CPG contained 0.5 % w/v TZC.

#### Introduce knockout vector into *Ralstonia* 
[Electroporation](electrocompetent_cells.md), [natural transformation](natural_transformation.md), and [conjugation](conjugation.md) are all possible strategies for introducing the vector into *Ralstonia*  

* Plate 200 μl of the transformed cells as well as 200 μl of the 10<sup>-1</sup>, 10<sup>-2</sup>, 10<sup>-3</sup> dilutions on CPG + Kan plates. Incubate at 28C for ~2 days. 

#### Isolate single recombinants ###
Isolate strains in which the allelic exchange vector has integrated at the chromosomal locus through a single crossover either at the upstream flank or the downstream flank.

