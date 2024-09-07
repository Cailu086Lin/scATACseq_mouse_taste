#  scATACseq_mouse_taste
Analysis provided in the manuscript titled "Inflammation causes bitter taste oversensitization via epigenetic changes in taste buds" 

This repository is meant to provide the source code for the analysis provided in the above manuscript by C Lin, M Jotaki, J Quinlan, S Feng, 
M Zhou, P Jiang, I Matsumoto, L Huang, Y Ninomiya, RF Margolskee, D Reed, H Wang

# Abstract

Chemosensory dysfunction often occurs with infection and cancer and contributes to food aversion and low quality of life. The underlying mechanisms of taste dysfunction, especially taste distortion, such as elevated and lingering bitter taste, are poorly understood. Here we report that, in an inflammation model mimicking bacterial infection, mice showed markedly heightened neural and behavioral responses to bitter compounds. Consistently, inflammation significantly up-regulated the expression of many Tas2r bitter receptor genes in taste tissues. Using single-cell assays for transposase-accessible chromatin with sequencing (scATAC-seq), we discovered that multiple Tas2r loci became more accessible during inflammation. Further scATAC-seq analyses revealed cell-type-specific chromatin accessibility of many taste-cell-selective genes and identified potential transcriptional regulators. Inflammation also induced substantial chromatin remodeling in immune response genes in taste tissue stem cells. Together, our results reveal an epigenetic mechanism connecting inflammation and altered bitter taste.


####
# sessionInfo()
R version 4.1.3 (2022-03-10)
Platform: x86_64-pc-linux-gnu (64-bit)
Running under: Ubuntu 20.04.4 LTS

Matrix products: default
BLAS:   /usr/lib/x86_64-linux-gnu/openblas-pthread/libblas.so.3
LAPACK: /usr/lib/x86_64-linux-gnu/openblas-pthread/liblapack.so.3

locale:
 [1] LC_CTYPE=en_US.UTF-8       LC_NUMERIC=C              
 [3] LC_TIME=en_US.UTF-8        LC_COLLATE=en_US.UTF-8    
 [5] LC_MONETARY=en_US.UTF-8    LC_MESSAGES=en_US.UTF-8   
 [7] LC_PAPER=en_US.UTF-8       LC_NAME=C                 
 [9] LC_ADDRESS=C               LC_TELEPHONE=C            
[11] LC_MEASUREMENT=en_US.UTF-8 LC_IDENTIFICATION=C       

attached base packages:
 [1] grid      parallel  stats4    stats     graphics  grDevices utils    
 [8] datasets  methods   base     

other attached packages:
 [1] uwot_0.1.11                        gridExtra_2.3                     
 [3] nabor_0.5.0                        Seurat_3.1.5                      
 [5] BSgenome.Mmusculus.UCSC.mm10_1.4.0 BSgenome_1.60.0                   
 [7] rtracklayer_1.52.1                 Biostrings_2.62.0                 
 [9] XVector_0.34.0                     ArchR_1.0.2                       
[11] magrittr_2.0.3                     rhdf5_2.38.1                      
[13] Matrix_1.4-1                       data.table_1.14.2                 
[15] SummarizedExperiment_1.24.0        Biobase_2.54.0                    
[17] GenomicRanges_1.46.1               GenomeInfoDb_1.30.1               
[19] IRanges_2.28.0                     S4Vectors_0.32.3                  
[21] BiocGenerics_0.40.0                MatrixGenerics_1.6.0              
[23] matrixStats_0.61.0                 ggplot2_3.3.5                     

loaded via a namespace (and not attached):
 [1] Rtsne_0.15               colorspace_2.0-3         rjson_0.2.21            
 [4] ellipsis_0.3.2           ggridges_0.5.3           farver_2.1.0            
 [7] leiden_0.3.9             listenv_0.8.0            ggrepel_0.9.1           
[10] RSpectra_0.16-0          fansi_1.0.3              codetools_0.2-18        
[13] splines_4.1.3            jsonlite_1.8.0           Rsamtools_2.8.0         
[16] Cairo_1.5-15             ica_1.0-2                cluster_2.1.3           
[19] png_0.1-7                sctransform_0.3.3        compiler_4.1.3          
[22] httr_1.4.2               assertthat_0.2.1         fastmap_1.1.0           
[25] lazyeval_0.2.2           cli_3.2.0                htmltools_0.5.2         
[28] tools_4.1.3              rsvd_1.0.5               igraph_1.3.0            
[31] gtable_0.3.0             glue_1.6.2               GenomeInfoDbData_1.2.7  
[34] RANN_2.6.1               reshape2_1.4.4           dplyr_1.0.8             
[37] Rcpp_1.0.8.3             vctrs_0.4.0              rhdf5filters_1.6.0      
[40] ape_5.6-2                nlme_3.1-157             lmtest_0.9-40           
[43] stringr_1.4.0            globals_0.14.0           lifecycle_1.0.1         
[46] irlba_2.3.5              restfulr_0.0.13          gtools_3.9.2            
[49] XML_3.99-0.9             future_1.24.0            zlibbioc_1.40.0         
[52] MASS_7.3-56              zoo_1.8-9                scales_1.1.1            
[55] RColorBrewer_1.1-3       yaml_2.3.5               reticulate_1.24         
[58] pbapply_1.5-0            stringi_1.7.6            BiocIO_1.2.0            
[61] BiocParallel_1.28.3      rlang_1.0.2              pkgconfig_2.0.3         
[64] bitops_1.0-7             lattice_0.20-45          ROCR_1.0-11             
[67] purrr_0.3.4              Rhdf5lib_1.16.0          labeling_0.4.2          
[70] GenomicAlignments_1.28.0 patchwork_1.1.1          htmlwidgets_1.5.4       
[73] cowplot_1.1.1            tidyselect_1.1.2         parallelly_1.30.0       
[76] RcppAnnoy_0.0.19         plyr_1.8.7               R6_2.5.1                
[79] generics_0.1.2           DelayedArray_0.20.0      DBI_1.1.2               
[82] pillar_1.7.0             withr_2.5.0              fitdistrplus_1.1-8      
[85] survival_3.3-1           RCurl_1.98-1.6           tibble_3.1.6            
[88] future.apply_1.8.1       tsne_0.1-3.1             crayon_1.5.1            
[91] KernSmooth_2.23-20       utf8_1.2.2               plotly_4.10.0           
[94] digest_0.6.29            tidyr_1.2.0              munsell_0.5.0           
[97] viridisLite_0.4.0  
