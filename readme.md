# Create a filtered reference panel from the 1000 Genomes Project Phase 3

Process

1. Obtain the 1000 Genome Project Phase 3 reference plnk2 file from https://www.cog-genomics.org/plink/2.0/resources#1kg_phase3
2. Only keep the biallelic snps on autosomes with a MAF > 0.01, geno > 0.95 and hwe > 1e-6 excluding the high LD regions. Remove by --mind 0.05 (nobody). Also align to hg38 refeerence and normalize. 
3. Exclude pallindromes and long LD regions were excluded. 
4. Rename the ID into chr:pos:ref:alt format
5. Create an ancestry mapping file

Please see the main.ipynb for the actual code.