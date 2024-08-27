SV Annotation Table Columns
---------------------------

This document describes each column in the SV Annotation Table.

**SV Name**: name of the SV.  

**Chromosome**: chromosome (chr1 to chr22, plus chrX, chrY, and chrM). 

**Start**: SV start. 

**End**: SV end. 

**Type**: SV types recognized by the pipeline are: duplications, deletions, inversions, and insertions. Insertions of size 1 are padded (+/- 50bp) prior to frequency calculations. BND are currently ignored. 

**Length**: length of the SV. 

**GC (%)**: GC content based on the UCSC genome reference GRCh38.  

**Cytoband**: cytoband. 

**Gene Count**: number of official gene symbol(s) for genes spanned by the SV based on the UCSC RefSeq gene definitions. 

**Gene Name(s)**: official gene symbol(s) for genes spanned by the SV based on the UCSC RefSeq gene definitions. 

**Gene at Start**: official gene symbol(s); overlap on SV start coordinate. 

**Gene at End**: official gene symbol(s); overlap on SV end coordinate. 

**Exon Name**: official gene symbol(s); exons overlap only. 

**CDS Name**: official gene symbol(s); coding exons overlap. 

**Dark Genes % Overlap**: % overlap with the dark regions from Twist Alliance.      

**ClinGen Haploinsufficient**: (array of) entrez gene ID, gene symbol, and score from the dosage sensitivity map, haploinsufficient phenotype defined in ClinGen. 

**ClinGen Triplosensitive**: (array of) entrez gene ID, gene symbol, and score for dosage sensitivity map, triplosensensitive phenotype defined in ClinGen. 

**gnomAD O/E LoF Upper**: observed/expected upper bound loss of function from gnomAD. 

**gnomAD O/E Mis Upper**: observed/expected upper bound missense from gnomAD. 

**gnomAD pLI**: probability that a gene falls into the class of intolerant of a single LoF gene (LoF- haploinsufficient intolerant genes), from gnomAD. 

**gnomAD pRec**: probability that a gene falls into the class of intolerant of two LoF genes (recessive genes), from gnomAD. 

**Repeat % Overlap**: percent overlap with repeat regions (RepeatMasker annotation from UCSC). 

**Dirty Region % Overlap**: percent overlap with gaps (including centromeres and telomeres), and segmental duplications 

**Chromosome Region**: telomere/centromere tag. 

**CGD**: (array of) entrez gene ID, gene symbol, disease name(s), and inheritance found in the Clinical Genomics Database; it is compiled by curators and maintained by the NHGRI (National Human Genome Research Institute); for every gene in the database, the CGD provides a list of one or more genetic disorders and a mode of inheritance (AD, AR, AD/AR, XL, more complex modes); since the CGD mode of inheritance is directly added by a curator and is tied to specific genetic disorder(s), it could be considered more accurate than the mode of inheritance for top-level HPO phenotypes. 

**OMIM Pheno**: (array of) entrez gene ID, gene symbol, and disorder/disease name(s), with their respective inheritance modes coded as “i:”, found in OMIM. 

**OMIM Inh**: list of all the inheritance modes for OMIM phenotypes. 
            autosomal dominant (AD), autosomal recessive (AR), multifactorial (MF), Y-linked (YL), X-linked dominant (XD), X-linked recessive (XR), X-linked: (XL), digenic recessive (DR), mitochondrial (MT), somatic mutation (SMu), somatic mosaicism (SMo), inherited chromosomal imbalance (ICI) 

**ClinGen Region**: Genomic disease region from ClinGen. 

**Decipher Region**: Genomic disease region from Decipher; the DatabasE of genomiC varIation and Phenotype in Humans using Ensembl Resources is an interactive web-based database which incorporates a suite of tools designed to aid the interpretation of genomic variants. For more information, see: https://decipher.sanger.ac.uk/. 

**ClinVar VarID**: ClinVar identifier. 

**gnomAD AF Max 90% RO**: highest allele frequencies among the subpopulation reported by gnomAD, with at least 90% reciprocal overlap. 

**gnomAD Population AF Max 90% RO**: subpopulation with the highest allele frequencies reported by gnomAD, with at least 90% reciprocal overlap. 

**gnomAD Hom/Ref Frequency 90% RO**: homozygous reference genotype frequency reported by gnomAD, with at least 90% reciprocal overlap. 

**gnomAD Het Frequency 90% RO**: heterozygous genotype frequency reported by gnomAD, with at least 90% reciprocal overlap. 

**gnomAD Hom/Alt Frequency 90% RO**: homozygous alternate genotype frequency reported by gnomAD, with at least 90% reciprocal overlap. 

**DGV % Overlap**: % length of SV overlapped by DGV region(s) (no cutoff used). The Database of Genomic Variants provides a comprehensive summary of structural variation in the human genome. For more information: http://dgv.tcag.ca/dgv. The DGV coordinates were lifted over to obtain the corresponding intervals in the GRCh38 reference genome. 

**DGV 50% RO**: % length covered by merged variants in DGV, restricted to those with at least 50% reciprocal overlap. 