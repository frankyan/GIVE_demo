# Long-range promoter contacts with capture Hi-C
This genome browser presents 4 datasets of long-range genome interactions along with human genome assembly GRCh37 (hg19) for comparative studies. These datasets were generated from a ***Nature Genetics*** paper [Borbala Mifsud et al., *Nature Genetics* 47, 598-606 (2015)](http://www.nature.com/ng/journal/v47/n6/full/ng.3286.html). They used Capture Hi-C (CHi-C), an adapted genome conformation assay, to examine the long-range interactions of almost 22,000 promoters in 2 human blood cell types, GM12878 and CD34<sup>+</sup>. They discovered different pattern and  promoter-promoter and promoter-other interactions were separated 

## Data Preparation
The processed significant long-range promoter contacts data in that paper can be downloaded from [E-MTAB-2323 of ArrayExpress](http://www.ebi.ac.uk/arrayexpress/files/E-MTAB-2323/E-MTAB-2323.additional.1.zip). 

``` bash
wget http://www.ebi.ac.uk/arrayexpress/files/E-MTAB-2323/E-MTAB-2323.additional.1.zip
unzip E-MTAB-2323.additional.1.zip
```
|chr | start | end | Symbol | Ensembl Gene ID | expresssion quartile | chr | start | end | Symbol | Ensembl Gene ID | expresssion quartile | raw count | log(observed/expected)|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|chr5|140556909|140558389|PCDHB8-001|ENSG00000120322|2|chr5|140558467|140562101|PCDHB16-201|ENSG00000196963|2|338|16.7349171319745|
|chr3|183266196|183267882|KLHL6-AS1-001|ENSG00000242522|1|chr3|183269400|183277960|KLHL6-001|ENSG00000172578|5|249|16.4555995112416|
|chr6|26238741|26244133|HIST1H4F-201|ENSG00000198327|5|chr6|26244367|26249842|HIST1H4G-201|ENSG00000124578|1|443|16.2749178680534|
|chr17|7512528|7516957|snoU13.445-201|ENSG00000251860|na|chr17|7516998|7519187|FXR2-201|ENSG00000129245|4|233|16.0225553055551|
|chr9|125232613|125235568|RP11-542K23.9-001|ENSG00000231465|1|chr9|125237734|125242999|OR1J1-201|ENSG00000136834|2|173|16.1066569764929|

There are 4 tracks in this genome browser, including significant promoter-promoter interactions and promoter-other interactions for both GM12878 and CD34+ cell types. We treat the promoter-other interactions as directed interactions, i.e., promoters are shown on the top genome and the interacted other genome regions are shown on the bottom genome. 
For questions, please contact Xiaoyi Cao (x9cao at ucsd dot edu). 
