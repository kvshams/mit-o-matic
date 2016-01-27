**Examples for command line**

```
1. Set default parameters: perl mitomatic.pl -c -i sample.fastq```

Runs complete pipeline with default parameters: alignment using maq, assuming data as single end, filtering variations with 10% hetereoplasmic frequency. Output is stored in folder named mitomatic\_out.

```
2. Change the alignment tool: perl mitomatic.pl -c -i sample.fastq -t bwa```

Runs complete pipeline using bwa for alignment, assuming data as single end, filtering variations with 10% hetereoplasmic frequency. Output is stored in folder named mitomatic\_out. To align with maq/bowtie, replace bwa with maq/bowtie.

```
3. Change the alignment tool and set frequency: perl mitomatic.pl -c -i sample.fastq -t bwa -f 5```

Runs complete pipeline using bwa for alignment, assuming data as single end, filtering variations with 5% hetereoplasmic frequency. Output is stored in folder named mitomatic\_out. Set frequency after option -f.

```
4. Change name of the output directory: perl mitomatic.pl -c -i sample.fastq -d sample_maq```

Runs complete pipeline using maq for alignment, assuming data as single end, filtering variations with 10% hetereoplasmic frequency. Output is stored in folder named sample\_maq.

```
5. For paired end data: perl mitomatic.pl -c -i sample_1.fastq sample_2.fastq -o pe```

Runs complete pipeline using maq for alignment considering paired end data, filtering variations with 10% hetereoplasmic frequency. Output is stored in folder named mitomatic\_out. In case -o pe option is not given, only the first file is considered for alignment, ignoring the second file.

```
6. For parsing already prepared pileup file: perl mitomatic.pl -p all.pileup -t bwa```

Filters variations with 10% heteroplasmic frequency from the pileup created by bwa and prepares a file parsed\_all.pileup compatible with mit-o-matic online version. -t option is mandatory while parsing pileup.

```
7. For parsing already prepared pileup file with a defined frequency: perl mitomatic.pl -p all.pileup -t maq -f 5```

Filters variations with 5% heteroplasmic frequency from the pileup created by maq and prepares a file parsed\_all.pileup compatible with mit-o-matic online version.