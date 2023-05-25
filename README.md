# sociogenomics


Instructions.
• Max 6 pages
• Include your names on the first page of the report
• Add your code (plink, R, or other) as an attachment to the
document (does not count in the 6 pages limit)
# Part 1. Work with genomics data
Use the files 1kg_hm3.bed, 1kg_hm3.bim, 1kg_hm3.fam
## 1.1. Using plink, select genetic variants and individuals that satisfy the following criteria (DONE)
- Variants with Minor Allele Frequency >0.05
- Individuals with genotyping rate >95%
- SNPs with call rate >95%
- SNPs for which HWE test is pvalue>0.00001
## (Todo: describe) 1.2. Describe the quality control procedure in 1.1.
##  1.3. Attach to the plink dataset a phenotype from the following files (DONE):
- height_sim.phen (group 1 )
- BMI_sim.phen (group 2)
- edu_sim.phen (group 3)
- Menarche_sim.phen (group 4)
## (todo: comment reults) 1.4. Use the resulting dataset and run a Additive Genome Wide Association Study using PLINK. Comment the results
## (todo:  make the description) 1.5. Report the first 10 SNPs with the smallest p-value. Describe the results
# Part 2. Polygenic risk score
## 2.1 Using the software PRSice-2 calculate a polygenic risk score. You can use as base dataset the plink files of part 1.1. As target file, you can use the following files:
- height.txt (group 1 )
- BMI.txt (group 2)
- Edu.txt (group 3)
- Menarche.txt (group 4)
Use the following options:
- Clumping 250kb, r2 =0.1
- Pvalue thresholding 5e-03, 5e-02, 5e-01 and 1

## 2.2. Describe 2.1 and the graphical outputs obtained.
 # Part 3. Work with summary statistics
## 3.1 Download from the GWAS Atlas the summary statistics from the most relevant and recent paper relative to your trait. Using R, prepare a Manhattan plot based on these summary statistics. 
Describe the plot.
## 3.2 Using the data in 3.1, prepare a QQplot. 
Describe the results.
## 3.3. From the GWAS Atlas website choose up to 10 traits related to your trait of interest and calculate their genetic correlations. Report them in a table or figure. 
Describe the results. 
