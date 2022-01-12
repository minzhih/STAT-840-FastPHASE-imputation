# STAT-840-FastPHASE-imputation-accury-evaluation-with-SeattleSNPs-data

#This project investigated the relationship between fastPHASE impu- tation accuracy and missing genotype rate in a small reference panel.


# The following steps are with modification, orgiranl step given by Professor: Lloyd Elliott
# Steps:

1. Read about fastPHASE here: Scheet, P and Stephens, M (2006). A fast and flexible statistical model for large-scale population genotype data: applications to inferring missing genotypes and haplotypic phase. Summarize this in your report. Get the fastPHASE software working and find the manual: https://faculty.washington.edu/browning/beagle/beagle.html

2. Download the SeattleSNPs data: https://pga.gs.washington.edu/data_download.html . Extract the HLA region.

3. For the HLA region, "mask" (i.e., hide, or remove) P = 10% of the genotypes (use whatever pattern of missingness is easiest to deal with in BEAGLE), and impute them using BEAGLE. Compare the computed values to the "ground truth" (i.e., the unhidden values). What was the percent correct for the imputation?

4. Vary P and report percent correct for BEAGLE's imputation.

I think this is achievable, but if you run into negative results or problems that you really can't solve, feel free to deviate from the path, or let me know and I'll chart a new path with you. Also, if you finish this and want to do more, you could do step 4 but with more than one method (i.e., compare BEAGLE to SHAPEIT4).

Accuracy = % of question marks that are filled in correctly.

Goals:

Question 1: How does accracy vary as %missing (missing at random) varies? Do some number of replicates per %missing condition. Vary %missing from 10% to 90%. a) For fastPHASE? (Achieved) b) For BEAGLE? 

Question 2: How do rare variants / reference panel mismatch affect %correct?

Question 3: Is there some kind of statistical method we could develop so that rare variants in the study panel can be detected? (Or more generally, if we KNOW there's a mismatch, can we do something to improve?) Maybe something can be done with the proir in a Bayseian model? Kind of like shrinkage.
