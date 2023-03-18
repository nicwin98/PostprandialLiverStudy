[![DOI](https://zenodo.org/badge/615819269.svg)](https://zenodo.org/badge/latestdoi/615819269)

# Postprandial Liver Study
This repository contains the bioinformatic analyses used to analyze RNA sequencing data from a study comparing human livers from:
- Healthy controls under fasting conditions
- Healthy controls under postprandial conditions
- NAFLD patients under fasting conditions
- NAFLD patients under postprandial conditions
- Cirrhosis patients under fasting conditions
- Healthy patients under postprandial conditions

## Data availability 
The raw FASTQ files and the salmon quant.sf files are available in the ArrayExpress database (http://www.ebi.ac.uk/arrayexpress) under accession numbers 
[E-MTAB-12807](https://www.ebi.ac.uk/arrayexpress/experiments/E-MTAB-12807)

## Session info for release v1.0.0
R version 4.2.0 (2022-04-22)
Platform: x86_64-apple-darwin17.0 (64-bit)
Running under: macOS Monterey 12.6.3

Matrix products: default
LAPACK: /Library/Frameworks/R.framework/Versions/4.2/Resources/lib/libRlapack.dylib

locale:
[1] da_DK.UTF-8/da_DK.UTF-8/da_DK.UTF-8/C/da_DK.UTF-8/da_DK.UTF-8

attached base packages:
[1] stats4    stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
 [1] plotly_4.10.1               shinythemes_1.2.0           shinyjs_2.1.0               shiny_1.7.3                 DT_0.26                    
 [6] EnhancedVolcano_1.14.0      GenomicFeatures_1.48.3      limma_3.52.2                ggpubr_0.4.0                writexl_1.4.1              
[11] xtable_1.8-4                repr_1.1.4                  clusterProfiler_4.4.4       org.Hs.eg.db_3.15.0         AnnotationDbi_1.58.0       
[16] DESeq2_1.36.0               SummarizedExperiment_1.26.1 Biobase_2.56.0              GenomicRanges_1.48.0        GenomeInfoDb_1.32.3        
[21] IRanges_2.30.0              S4Vectors_0.34.0            BiocGenerics_0.42.0         MatrixGenerics_1.8.1        matrixStats_0.62.0         
[26] genefilter_1.78.0           hexbin_1.28.2               ggrepel_0.9.1               RColorBrewer_1.1-3          viridis_0.6.2              
[31] viridisLite_0.4.1           pheatmap_1.0.12             forcats_0.5.2               stringr_1.4.1               dplyr_1.0.10               
[36] purrr_0.3.5                 readr_2.1.3                 tidyr_1.2.1                 tibble_3.1.8                ggplot2_3.4.0              
[41] tidyverse_1.3.2             tximeta_1.14.1             

loaded via a namespace (and not attached):
  [1] rappdirs_0.3.3                rtracklayer_1.56.1            bit64_4.0.5                   knitr_1.40                   
  [5] DelayedArray_0.22.0           data.table_1.14.4             KEGGREST_1.36.3               RCurl_1.98-1.9               
  [9] AnnotationFilter_1.20.0       generics_0.1.3                RSQLite_2.2.18                shadowtext_0.1.2             
 [13] bit_4.0.4                     tzdb_0.3.0                    enrichplot_1.16.1             xml2_1.3.3                   
 [17] lubridate_1.9.0               httpuv_1.6.6                  assertthat_0.2.1              fontawesome_0.4.0            
 [21] gargle_1.2.1                  xfun_0.34                     tximport_1.24.0               hms_1.1.2                    
 [25] jquerylib_0.1.4               evaluate_0.17                 promises_1.2.0.1              fansi_1.0.3                  
 [29] restfulr_0.0.15               progress_1.2.2                dbplyr_2.2.1                  readxl_1.4.1                 
 [33] igraph_1.3.5                  DBI_1.1.3                     geneplotter_1.74.0            htmlwidgets_1.5.4            
 [37] googledrive_2.0.0             ellipsis_0.3.2                crosstalk_1.2.0               backports_1.4.1              
 [41] annotate_1.74.0               biomaRt_2.52.0                vctrs_0.5.0                   ensembldb_2.20.2             
 [45] abind_1.4-5                   cachem_1.0.6                  withr_2.5.0                   ggforce_0.4.1                
 [49] vroom_1.6.0                   GenomicAlignments_1.32.1      treeio_1.20.1                 prettyunits_1.1.1            
 [53] DOSE_3.22.0                   ape_5.6-2                     lazyeval_0.2.2                crayon_1.5.2                 
 [57] pkgconfig_2.0.3               labeling_0.4.2                tweenr_2.0.2                  nlme_3.1-160                 
 [61] ProtGenerics_1.28.0           rlang_1.0.6                   lifecycle_1.0.3               downloader_0.4               
 [65] filelock_1.0.2                BiocFileCache_2.4.0           modelr_0.1.9                  AnnotationHub_3.4.0          
 [69] cellranger_1.1.0              polyclip_1.10-4               Matrix_1.5-1                  aplot_0.1.8                  
 [73] carData_3.0-5                 reprex_2.0.2                  base64enc_0.1-3               googlesheets4_1.0.1          
 [77] png_0.1-7                     rjson_0.2.21                  bitops_1.0-7                  Biostrings_2.64.0            
 [81] blob_1.2.3                    qvalue_2.28.0                 rstatix_0.7.0                 gridGraphics_0.5-1           
 [85] ggsignif_0.6.4                scales_1.2.1                  memoise_2.0.1                 magrittr_2.0.3               
 [89] plyr_1.8.7                    zlibbioc_1.42.0               compiler_4.2.0                scatterpie_0.1.8             
 [93] BiocIO_1.6.0                  Rsamtools_2.12.0              cli_3.4.1                     XVector_0.36.0               
 [97] patchwork_1.1.2               MASS_7.3-58.1                 mgcv_1.8-41                   tidyselect_1.2.0             
[101] stringi_1.7.8                 yaml_2.3.6                    GOSemSim_2.22.0               locfit_1.5-9.6               
[105] grid_4.2.0                    sass_0.4.2                    fastmatch_1.1-3               tools_4.2.0                  
[109] timechange_0.1.1              parallel_4.2.0                rstudioapi_0.14               gridExtra_2.3                
[113] farver_2.1.1                  ggraph_2.1.0                  digest_0.6.30                 BiocManager_1.30.19          
[117] Rcpp_1.0.9                    car_3.1-1                     broom_1.0.1                   BiocVersion_3.15.2           
[121] later_1.3.0                   httr_1.4.4                    rsconnect_0.8.28              colorspace_2.0-3             
[125] rvest_1.0.3                   XML_3.99-0.12                 fs_1.5.2                      splines_4.2.0                
[129] yulab.utils_0.0.5             tidytree_0.4.1                graphlayouts_0.8.3            ggplotify_0.1.0              
[133] jsonlite_1.8.3                ggtree_3.4.1                  tidygraph_1.2.2               ggfun_0.0.7                  
[137] R6_2.5.1                      pillar_1.8.1                  htmltools_0.5.3               mime_0.12                    
[141] glue_1.6.2                    fastmap_1.1.0                 BiocParallel_1.30.3           interactiveDisplayBase_1.34.0
[145] codetools_0.2-18              fgsea_1.22.0                  utf8_1.2.2                    lattice_0.20-45              
[149] bslib_0.4.1                   curl_4.3.3                    GO.db_3.15.0                  survival_3.4-0               
[153] rmarkdown_2.17                munsell_0.5.0                 DO.db_2.9                     GenomeInfoDbData_1.2.8       
[157] haven_2.5.1                   reshape2_1.4.4                gtable_0.3.1
