# ssGSEA2.0/PTM-SEA



Resources for gene-centric **single sample Gene Set Enrichment Analysis (ssGSEA)** of gene expression data (e.g. mRNAs, proteins) and site-centric **PTM Signature Enrichment Analysis (PTM-SEA)** [1] of phosphoproteomics data sets using the [**PTM signatures database (PTMsigDB)**](http://prot-shiny-vm.broadinstitute.org:3838/ptmsigdb-app/) [1].


## Disclaimer

The primary purpose of this repository is to supplement our [manuscript](https://www.mcponline.org/content/18/3/576.abstract) in which we describe PTM-SEA and [PTMsigDB](http://prot-shiny-vm.broadinstitute.org:3838/ptmsigdb-app/). While ssGSEA2.0 presents an updated version of the original ssGSEA R implementation, we want to acknowledge that this is not the primary repository for ssGSEA. The official codebase for ssGSEA can be found [here](https://github.com/GSEA-MSigDB/ssGSEA-gpmodule), and the official GenePattern module to perform ssGSEA can be accessed [here](https://www.genepattern.org/modules/docs/ssGSEAProjection/4).


## ssGSEA 2.0

This is an updated version of the original ssGSEA [2,3] R-implementation. Depending on the input dataset and chosen database (gene sets or PTM signatures), the software performs either ssGSEA or PTM-SEA, respectively. The Molecular Signatures Database ([MSigDB](http://software.broadinstitute.org/gsea/msigdb/)) [4] provides a large collection of curated gene sets.  Gene sets are stored as plain text in  [GMT](https://software.broadinstitute.org/cancer/software/gsea/wiki/index.php/Data_formats#GMT:_Gene_Matrix_Transposed_file_format_.28.2A.gmt.29) format. A current version of MSigDB gene set collections can be found in the ```db/msigdb``` subfolder. MSigDB gene sets are realeased under [Creative Commons Attribution 4.0 International License](http://software.broadinstitute.org/gsea/msigdb_license_terms.jsp). The license terms can be found in the```db/msigdb``` folder.

File formats supported by ssGSEA2.0/PTM-SEA are Gene Cluster Text [GCT v1.2](https://software.broadinstitute.org/cancer/software/gsea/wiki/index.php/Data_formats#GCT:_Gene_Cluster_Text_file_format_.28.2A.gct.29) or [GCT v1.3](https://clue.io/connectopedia/gct_format) files. [Morpheus](https://software.broadinstitute.org/morpheus/) provides a convenient way to convert your data tables into GCT format.

For more information about the GSEA method and MSigDB please visit http://software.broadinstitute.org/gsea/.


## How can I use these tools?

I modified the GUI version to a R script named "main.R" that will generate ssGSEA results.     
Remember to modify directory paths in "main.R", MsigDB files and .gct files.



## License
License Agreement for MSigDB v6.0 and above can be found [here](https://raw.githubusercontent.com/broadinstitute/ssGSEA2.0/master/db/msigdb/license.txt).

## References
1.  Krug, K., Mertins, P., Zhang, B., Hornbeck, P., Raju, R., Ahmad, R., . Szucs, M., Mundt, F., Forestier, D., Jane-Valbuena, J., Keshishian, H., Gillette, M. A., Tamayo, P., Mesirov, J. P., Jaffe, J. D., Carr, S. A., Mani, D. R. (2019). **A curated resource for phosphosite-specific signature analysis**, Molecular & Cellular Proteomics (in Press). http://doi.org/10.1074/mcp.TIR118.000943

1.  Barbie, D. A., Tamayo, P., Boehm, J. S., Kim, S. Y., Susan, E., Dunn, I. F., . Hahn, W. C. (2010). **Systematic RNA interference reveals that oncogenic KRAS- driven cancers require TBK1**, Nature, 462(7269), 108-112. https://doi.org/10.1038/nature08460

1. Abazeed, M. E., Adams, D. J., Hurov, K. E., Tamayo, P., Creighton, C. J., Sonkin, D., et al. (2013).
       **Integrative Radiogenomic Profiling of Squamous Cell Lung Cancer.** Cancer Research, 73(20), 6289-6298.
       http://doi.org/10.1158/0008-5472.CAN-13-1616

1. Subramanian, A., Tamayo, P., Mootha, V. K., Mukherjee, S., Ebert, B. L., Gillette, M. A., et al. (2005).
   **Gene set enrichment analysis: a knowledge-based approach for interpreting genome-wide expression profiles.**
  Proceedings of the National Academy of Sciences of the United States of America, 102(43), 15545-15550. http://doi.org/10.1073/pnas.0506580102

1. Hornbeck, P. V., Zhang, B., Murray, B., Kornhauser, J. M., Latham, V., & Skrzypek, E. (2015). **PhosphoSitePlus, 2014: mutations, PTMs and recalibrations.** Nucleic Acids Research, 43(D1), D512-D520. https://doi.org/10.1093/nar/gku1267
 

1. Cox, J., & Mann, M. (2008). **MaxQuant enables high peptide identification rates, individualized p.p.b.-range mass accuracies and proteome-wide protein quantification.** Nature Biotechnology, 26(12), 1367-1372. https://doi.org/10.1038/nbt.1511


1. Reich, M., Liefeld, T., Gould, J., Lerner, J., Tamayo, P., & Mesirov, J. P. (2006). **GenePattern 2.0.** Nature Genetics, 38(5), 500-501. https://doi.org/10.1038/ng0506-500


***
