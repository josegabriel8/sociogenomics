# Part 1 (Everything should work just copy and pasting)

## For Install plink, (I installed it in the $HOME directory)
wget https://s3.amazonaws.com/plink1-assets/plink_linux_x86_64_20230116.zip
unzip plink_linux_x86_64_20230116.zip
chmod +x plink

## 1-Create two directories:
mkdir Final_project_data
mkdir Final_project_results

## 2- Create a link in the data directory for plink:
cd $HOME/Final_project_data
ln -s $HOME/plink

## 4- Upload the files “1kg_hm3.bed, 1kg_hm3.bim, 1kg_hm3.fam” (put them inside Final_project_data directory)

## 5-Filtering of variants and individuals:
./plink --bfile 1kg_hm3 --maf 0.05 --mind 0.05 --geno 0.05 --hwe 0.00001 --make-bed --out filtered_data

## 6- Upload the file “edu_sim.phen” in the same directory.

## 7- Attach phenotype:
./plink --bfile filtered_data --pheno edu_sim.phen --make-bed --out final_data

## 8-Create results.
plink --bfile final_data --assoc --out $HOME/ Final_project_results /gwas_results

## 9-Selecting the 10 variants with smaller P-value:
sort -g -k9,9 gwas_results.qassoc | head -n 11 > filtered_gwasresults.txt

