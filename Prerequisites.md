**Raw sequencing reads:** Mitochondrial DNA sequence data is stored in fastq format which reports nucleotide sequence with their Phred qualities in a single file. Offline version is compatible with data having 51 bp of read length.

**Reference genome:** The analysis is based on alignment of sequencing reads with modified version of revised Cambridge Reference Genome Sequence (rCRSm) which can be downloaded from http://genome.igib.res.in/mitomatic/

**Alignment tool:** MAQ, BWA or BOWTIE can be used for sequence alignment and variant calling. Pileup file summarizes the base calls of aligned reads to a reference sequence and is required to extract variations in the sample reads.

**Offline version:** The script (mitomatic\_offline.pl) provided in the offline version can be used either to run the complete computational pipeline or to parse the pileup file created by MAQ, BWA or BOWTIE. The parsed file is can be uploaded to mit-o-matic (http://genome.igib.res.in/mitomatic/) for further analysis.