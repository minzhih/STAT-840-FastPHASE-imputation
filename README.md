# STAT-840-FastPHASE-imputation-accury-evaluation-with-SeattleSNPs-data

### Note :I spotted errors in my Abstract and Introduction, as well as in the Methodology part. It's a small try for me to learn about research and statistical genetics. The writing, research steps, code, and report could all be better and more complete.
New report revising.


#This project investigated the relationship between fastPHASE imputation accuracy and missing genotype rate in a small reference panel. Note :  I spotted there was an error in my data descrpbtion and HLA extraction. I extracted the TNF region in my oraginal report. New report revising.

# The orgiranl step given by Professor: Lloyd Elliott
# Steps:
1. Read about fastPHASE here: Scheet, P and Stephens, M (2006). A fast and flexible statistical model for large-scale population genotype data: applications to inferring missing genotypes and haplotypic phase. Summarize this in your report. Get the fastPHASE software working and find the manual: https://faculty.washington.edu/browning/beagle/beagle.html

2. Download the SeattleSNPs data: https://pga.gs.washington.edu/data_download.html. Extract the HLA region (included in HLA): https://pga.gs.washington.edu/data/tnf/.

3. For the HLA region, "mask" (i.e., hide, or remove) P = 10% of the genotypes (use whatever pattern of missingness is easiest to deal with in BEAGLE), and impute them using BEAGLE. Compare the computed values to the "ground truth" (i.e., the unhidden values). What was the percent correct for the imputation?

4. Vary P and report percent correct for fastPHASE's imputation.

Accuracy = % of question marks that are filled in correctly.

Goals:
Question 1: How does accracy vary as %missing (missing at random) varies? Do some number of replicates per %missing condition. Vary %missing from 10% to 90%. For fastPHASE? (Achieved)  

Question 2: How do rare variants / reference panel mismatch affect %correct?

Question 3: Is there some kind of statistical method we could develop so that rare variants in the study panel can be detected? (Or more generally, if we KNOW there's a mismatch, can we do something to improve?) Maybe something can be done with the proir in a Bayseian model? Kind of like shrinkage.

Example report page:

<img width="958" alt="Screen Shot 2022-12-23 at 4 21 38 PM" src="https://user-images.githubusercontent.com/37996767/209415041-b3dfbe0d-f4b3-4ec6-a7ac-093d0a56fbd3.png">


