illumina-pipeline
=================

Diversity estimation pipeline for high-throughput sequencing (Illumina) platforms. This pipeline has been used for analysis of foraminiferal and eukaryotic diversity in

* F Lejzerowicz, P Esling, W Majewski, W Szczuciński, J Decelle, C Obadia, PM Arbizu, J Pawlowski, "Ancient DNA complements microfossil record in deep-sea subsurface sediments", *Biology Letters*, vol.9, no.4, 2013.
* P Esling, F Lejzerowicz, J Pawlowski "High-throughput accuracy for multiplex amplicon sequencing", *Nature Methods*, in review.
* J Pawlowski, P Esling, F Lejzerowicz, T Cedhagen, T Wilding "Environmental monitoring through protist NGS metabarcoding: assessing the impact of fish farming on benthic foraminifera communities", *Molecular Ecology Resources*, in review.

This pipeline has been developped in C language for fast processing. In order to use the pipeline on raw (FASTQ) data, prior to the publication and disclosure of its inner methods, we pre-compiled the software for different architectures. Hence, you can find here the executables for the pipeline
* **illuminaPipeline-Unix**
* **illuminaPipeline-MacOS**

In all cases, we will refer to these executables as **illuminaPipeline** in the following.

In order to produce an output of assembly, diversity estimation and statistics, the program should be called in the following manner (in a terminal window)

./illuminaPipeline **-forwardFile** *\<Path to R1 FastQ\>* **-reverseFile** *\<Path to R1 FastQ\>*  **-taggingFile** *\<Path to list of tags (fasta)\>* **-outputDir** *\<Path to directory for results\>*  **-meanQual** *\<Mean read Q (int)\>*  **-minBase** *\<Minimum Q of a base\>* **-maxAmb** *\<Maximum number of ambiguous\>* **-primMiss** *\<Number of errors in primer\>* **-tagMiss** *\<Number of errors in tag\>* **-taxonomyFile** *\<Path to taxonomy database (fasta)\>*

This git-hub repository will also be re-used once the pipeline has been fully disclosed in order to provide the community with the complete source code, so stay in touch.
