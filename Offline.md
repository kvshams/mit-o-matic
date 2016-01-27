Offline platform of mit-o-matic offers execution of the entire computational pipeline with a single command. The script provided runs alignment of the sample reads on the modified reference genome (rCRSm) using the selected platform (MAQ, BWA or BOWTIE). Pileup file generated is then parsed to extract and filter variations based on heteroplasmic frequencies. Finally the parsed pileup is submitted to http://genome.igib.res.in/mitomatic/ with LWP. This generates a sample report in the form of an html file (mito\_out.html) in the output directory.

The user can use the same script to just parse an already created pileup and save it for future use for analysis of mitochondrial variations with mit-o-matic. Different heteroplasmic frequencies can be set depending on the depth of sample reads. Usually 10% heteroplasmic frequency is considered to be acceptable.

## Untar the downloaded file: ##
```
 tar -xvzf mitomatic_command-line.tar.gz```

## Change directory: ##
```
cd mitomatic_command-line```

## For 32-bit CPU Architecture: ##
```
 mv bin-32 bin```

## For 64-bit CPU Architecture: ##
```
mv bin-64 bin```

## Complete pipeline ##
```

USAGE: perl mitomatic_offline.pl -t [bowtie/bwa/maq] -o [se/pe] -f [Percentage of heteroplasmic frequency] -d [output directory] -i [input fastq files]
```
## Parsing pileup ##
```

USAGE: mitomatic_offline.pl -p [pileup file] -t [bowtie/bwa/maq] -f [Percentage of heteroplasmic frequency]```

```


-t Tool to be used for the alignment from BWA, BOWTIE and MAQ
-o Type of data, whether single end or paired end
-f Percentage of heteroplasmic frequency to call the variants [Preferred: 10]
-d Name of the output directory
-I Input fastq file. In case of paired end data mention both the files one after other
-p For parsing an already generated pileup

-h Help
```