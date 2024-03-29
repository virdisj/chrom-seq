# chrom-seq


**Python pipeline for ATAC-seq and ChIP-seq analysis**

Install following tools and setup in your path (except picard.jar):

bowtie2: https://sourceforge.net/projects/bowtie-bio/files/bowtie2/2.5.3/

MACS2: https://pypi.org/project/MACS2/

PICARD: https://broadinstitute.github.io/picard/

samtools: http://www.htslib.org/download/ 

docopt: https://github.com/docopt/docopt


**usage:**

chrom-seq.py -h 

**example:**

```
chrom-seq.py align-pe sample_read1.fastq.gz sample_read2.fastq.gz ~/Desktop/ref/Bowtie2Index -t 3 -o test.bam

chrom-seq.py dedup-shift test_sorted.bam ~/Desktop/tools/ -t 6 --atac

chrom-seq.py call-peaks test_sorted_dedup.bam test peaks --atac
```
