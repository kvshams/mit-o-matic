## Pileup Format ##

It is a text-based format for describing the base-pair information of the reads aligned to a reference sequence. It facilitates the display of SNP/Indel calling and alignment as well. Each line consists of 5-6 tab separated columns that include Sequence identifier, position in sequence (1-based coordinate system), reference base, number of reads covering the site (depth of coverage), read bases and base qualities.

### Format Description ###
http://genome.igib.res.in/mitomatic/fig2.PNG


## Parsed pileup Format for mit-o-matic ##

The input for mit-o-matic is a tab-delimited file, prepared from the pileup file. Each line consists of a sequence identifier, position, reference base, number of reads covering the site (depth of coverage), count of A, T, G, C nucleotides, number of forward and reverse reads, counts of nucleotides in forward and reverse strands repectively. To prepare the input file for mit-o-matic in this format, a perl script (mitomatic\_offline.pl) has been provided in the offline version available at the home page.
Use offline version of mit-o-matic to parse the pileup file
```

USAGE: mitomatic_offline.pl -p [pileup file] -t [bowtie/bwa/maq] -f [Percentage of heteroplasmic frequency]
```

### Format Description ###
![http://genome.igib.res.in/mitomatic/tab2.jpg](http://genome.igib.res.in/mitomatic/tab2.jpg)

### Sample Pileup ###
![http://genome.igib.res.in/mitomatic/tab1.jpg](http://genome.igib.res.in/mitomatic/tab1.jpg)