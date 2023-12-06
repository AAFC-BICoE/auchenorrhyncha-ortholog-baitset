# *Hemiptera:Auchenorrhyncha* Ortholog Target Enrichment Baits

The 2017 Hemipteran Bait set provided by Christopher H. Dietrich and Yanghui Cao contains 56854 baits targeting 498 orthogroups. This is 16854 baits higher than Arbor Biosciences MyBait manufacturing tier of 40000. This project reduces the size of the bait while preserving the number of orthogroups and the focus on Auchenorrhyncha.

### Acknowledgements

Developed under the direction of Jeremy Dettman as part of BioMob WP2

This bait set was made possible by the significant contributions from the following scientists:

- Christopher H. Dietrich and Yanghui Cao for providing aligned orthologs from the 2017 baitset
- Dr. Joel Kits for the phylogenetic expertise to reduce the bait set size while preserving effectiveness
- Dr. Jeremy Dettman, Julie Chapados, Robin Richter, Wayne McCormick (Agriculture & Agri-Food Canada) for the extensive validation and implementing of the bait set.

### Design Methodology

* 498 Aligned orthologs were provided by Christopher H. Dietrich and Yanghui Cao. However the information only indicated if the genetic data came from a genome or a transcriptome and lacked species identifiers
* To identify species, genome baits were blasted against NCBI's database with results available in Probe_Blast_Results.txt
* The 498 orthologs were concatenated into a Phylip file and processed with IQTree to generate a general phylogeny
* This Phylogeny was examined by Dr. Joel Kits along with the previous blast data. 
The identified species allowed the tree to be colour coded into a generally accepted Phylogeny of *Hemiptera*
* With each species generally identified, the order of baits to remove was Psocodea, Thysanoptera, Sternorrhyncha, then Heteroptera in order to preserve as many Auchenorrhynca baits as possible
* 32 Representative species were removed corresponding to Psocodea, Thysanoptera, Sternorrhyncha and encompassing 17075 baits
* The final bait set was converted into Phyluce compatible UCE format for processing the [AAFC partial-genome-pipeline](https://github.com/AAFC-BICoE/snakemake-partial-genome-pipeline)
* In order to evaluate the theoretical performance of the bait set, it was compared against a Hemipteran transcriptomes from the Short Read Archive

|     Specimen      |     Merged Targets    |
|-------------------|-----------------------|
|     SRR5988590    |     404               |
|     SRR5988592    |     366               |
|     SRR5988589    |     368               |
|     SRR5988595    |     370               |
|     SRR5988599    |     388               |
|     SRR5988594    |     389               |
|     SRR5988591    |     376               |
|     SRR5988593    |     381               |
|     SRR5988596    |     202               |
|     SRR5988597    |     365               |
|     SRR5988598    |     347               |

These results are similar to the experimental performance of the original baitset. 

* The final bait set contains 39779 baits targeting 498 orthogroups 

### Built With

* [Python](https://www.python.org/doc/) - Programming language
* [Conda](https://conda.io/docs/index.html) - Package, dependency and environment management
* [Phyluce](https://phyluce.readthedocs.io/en/latest/index.html) - Target enrichment data analysis
* [BioPython](https://biopython.org/) - Tools for biological computation


### Contact
Jackson Eyres, Bioinformatics Programmer, Agriculture & Agri-Food Canada  
jackson.eyres@canada.ca

### Cite Us

If you use this bait set, please cite the following paper

Yanghui Cao, Christopher H Dietrich, Joel H Kits, Dmitry A Dmitriev, Robin Richter, Jackson Eyres, Jeremy R Dettman, Ye Xu, Min Huang, Phylogenomics of microleafhoppers (Hemiptera: Cicadellidae: Typhlocybinae): morphological evolution, divergence times, and biogeography, *Insect Systematics and Diversity*, Volume 7, Issue 4, July 2023, 1, https://doi.org/10.1093/isd/ixad010

### Copyright

Agriculture & Agri-Food Canada, Government of Canada

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

### Citations

1. Yanghui Cao, Christopher H Dietrich, Joel H Kits, Dmitry A Dmitriev, Robin Richter, Jackson Eyres, Jeremy R Dettman, Ye Xu, Min Huang, Phylogenomics of microleafhoppers (Hemiptera: Cicadellidae: Typhlocybinae): morphological evolution, divergence times, and biogeography, *Insect Systematics and Diversity*, Volume 7, Issue 4, July 2023, 1, https://doi.org/10.1093/isd/ixad010

2. Faircloth BC. 2016. PHYLUCE is a software package for the analysis of conserved genomic loci. Bioinformatics 32:786-788. doi:10.1093/bioinformatics/btv646.

