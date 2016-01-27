**Report Summary:**

The tool summarizes the report of analysis on top of the output page. Herein, the reference genome being used, the haplogroup corresponding to the input variants and counts of some significant characteristics of the report are described. This includes:

![http://genome.igib.res.in/mitomatic/fig3.png](http://genome.igib.res.in/mitomatic/fig3.png)

|Reference sequence: |Reference genome that has been used for analysis|
|:-------------------|:-----------------------------------------------|
|Number of Variants Uploaded: |Count of the variants that have been uploaded by the user|
|Number of Variants Mapped: |Count of the variants that have already been reported in the widely used databases that include mitomap and mtDB.|
|Novel Variants:     |The variants that have not been reported as of now in the available databases are considered to be novel.|
|Haplogroup:         |It reports the haplogroup to which the uploaded variants belong. This is deciphered from the haplogroup table compiled from the comprehensive phylogenetic tree of global human mitochondrial DNA variation (available at http://www.phylotree.org/builds/mtDNA_tree_Build_15.zip). The haplogroup having the highest number of variants matching to the input variants is reported.|
|Disease Associated Variants: |Number of variants that have been reported to have association with some mitochondrial disease by mitomap (available at http://www.mitomap.org/bin/view.pl/MITOMAP/MutationsCodingControl)|
|Number of Heteroplasmic Sites: |Number of times multiple mutations co-exist in various proportions (>10%) within the mitochondrial DNA.|
|Number of Variants with Population Frequency: |It reports the count of variants for which population frequency could be found. |

Below the report summary three different panels give section-wise information regarding annotation of individual variation. Certain parameters common to each panel include variant position, heteroplasmy percentage, reference allele, alternate allele, amino acid change corresponding to mutation, gene within which the variant position falls, type of mutation and population frequency for the variant. In case more than one mutations co-exist in various proportions (>10%) within the mitochondrial DNA, the site is considered to be heteroplasmic and is marked with a **sign.**

Nucleotides for which Heteroplasmy percentage is greater than 10% are considered to be the alternate alleles and are reported along with the corresponding percentage in the second column.

**_Heteroplasmy percentage = (Number of A/T/G/C x 100)/Total Number of Reads_**

**Description of column names:**

|Column Name|Description|
|:----------|:----------|
|Variant    |Variant Position|
|Heteroplasmy %|Percentage of heteroplasmic frequency|
|Ref Allele |Reference Allele|
|Alt Allele |Alternate Allele|
|AA Position|Amino Acid Position|
|AA Change  |Change in Amino Acid|
|Gene       |Mitochondrial DNA Function Location (Gene Loci)|
|Disease    |Associated Disease|
|Syn/Non-Syn|Type of mutation - Synonymous or Non - Synonymous|
|Pop Freq   |Population Frequency|
|Homoplasmy |'+' If Homoplasmic at variant position|
|Heteroplasmy|'+' If Heteroplasmic at variant position|
|SIFT Prediction|Whether the non-synonymous mutation is Tolerated or Deleterious|

**Phenotype Association panel:**

All the variations that are associated with phenotype and thus have disease association are reported under this panel. 8th column reports the corresponding disease that might be seen in case of variation at that particular position.

![http://genome.igib.res.in/mitomatic/fig4.png](http://genome.igib.res.in/mitomatic/fig4.png)

**Novel Variants panel:**

All the variations that are not reported in any other database as of now are considered to be novel and their corresponding information is shown within this panel. SIFT annotations are provided for the non-synonymous novel variants to analyze the effect of amino acid substitution on the protein function based upon structural change in protein.

![http://genome.igib.res.in/mitomatic/fig5.png](http://genome.igib.res.in/mitomatic/fig5.png)

**Mapped Variants panel:**

This panel enlists information regarding those variations that have already been reported in any of the existing databases. Position 3107, represented by an "N" is the error nucleotide in the original CRS that is maintained in the revised sequence as a gap. This error position shall always be detected as one of the heteroplasmic sites.

![http://genome.igib.res.in/mitomatic/fig6.png](http://genome.igib.res.in/mitomatic/fig6.png)

