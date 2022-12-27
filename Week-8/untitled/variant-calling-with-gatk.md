---
description: This page takes an estimated 45 minutes to complete.
---

# Variant Calling With GATK

**Variant calling** entails identifying single nucleotide polymorphisms (SNPs) and small insertions and deletion (indels) from NGS data.

## Help Material

For this page, you will use the [Variant Calling with GATK website ](https://learn.gencore.bio.nyu.edu/variant-calling/)and the presentation below as help material.

{% embed url="https://docs.google.com/presentation/d/1Mq7YWGz-PK9myvNl52MHNavK_SYCXWf3GQAUiO6wxlA/edit#slide=id.p" %}

## Tutorial

1. Copy _**variant\_calling\_files.tar.gz**_ archive from **/home/shared/ngs\_data/variant\_calling** folder to your home directory and extract files from the archive.
2. In the [Pre-Processing](https://learn.gencore.bio.nyu.edu/variant-calling/pre-processing/) step, please skip the **“Setting up your environment..”** parts and start from **“1) Alignment”**, as we already have a ready environment in our server. Please also skip the **“6) Base Quality Score Recalibration”** section.
3. Read the tutorial run the commands from the _**variant\_calling\_script.sh**_ file according to the steps in the tutorial (commands presented in this tutorial will not work in your server as the software and input data are different)
4. In the [Variant discovery](https://learn.gencore.bio.nyu.edu/variant-calling/variant-discovery/) section skip the **“3) Annotation”** part. For the visualization of the results in the IGV (Integrative genomic viewer) browser, you should [download](https://software.broadinstitute.org/software/igv/download) and install IGV on your computer.
5. After successfully running all commands from the _**variant\_calling\_script.sh**_ file you should get filtered .vcf files for SNPs and Indels. For visualization of calculated results download these files to your computer:
   * dedup\_reads.bam
   * dedup\_reads.bam.bai
   * filtered\_snps.vcf
   * filtered\_snps.vcf.idx
   * ecoli\_rel606.fasta
6. Open IGV browser in your computer and load downloaded _**ecoli\_rel606.fasta**_ genome via Genomes > “Load Genom from file…”.&#x20;
7. Now you can load bam and .vcf files via File > “Load from file…”. You can check mutations and navigate through the genome by inserting coordinates on top of the window (example coordinate: CP000819.1:2,446,706-2,447,373)

## Congratulations!

If you made it here, then congratulations! You have successfully completed this section. Move to the next portion of the guide with the arrow buttons below.
