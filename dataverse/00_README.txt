# README


# DESCRIPTION
This repository contains original data from a survey collecting information about the use of toothpastes in Latvia and Lithuania. The analysis script is included.  The dataset also includes a statistical analysis script, created using the R software, and specifications for reproducing the analysis. Additionally, a codebook is included to explain the different codes used in the data. The data was obtained from a survey research and has been appropriately anonymized for use in research. To ensure compliance with FAIR data principles, the data is clearly documented and the data management process is well-described, the data is accessible and reusable, and the data is properly cited.

=============
# CONTACT
Sergio Uribe, sergio.uribe@rsu.lv

============
# AUTHORS
Ilze Maldupa1,Julija Narbutaite2, Egle Stanceviciene2, Ilona Viduskalne1, Julija Kalnina, Liga Kronina, Anda Brinkmane1, Egita Senakola1, Sergio E. Uribe1, 3, 4

1 Department of Conservative Dentistry and Oral Health, Riga Stradins University, Riga, Latvia
2 Lithuanian University of Health Sciences, Kauna, Lithuania 
3 Baltic Biomaterials Centre of Excellence, Headquarters at Riga Technical University, Riga, Latvia
4 School of Dentistry, Universidad Austral de Chile, Valdivia, Chile

Ilze Maldupa 0000-0002-5967-956X
Julija Narbutaite 0000-0002-5156-3861
Egle Stanceviciene
Ilona Viduskalne 0000-0001-6193-2205
Julija Kalnina
Liga Kronina
Anda Brinkmane 0000-0003-1843-0423
Egita Senakola 0000-0002-6422-9061
Sergio E. Uribe  0000-0003-0684-2025

=============
# FILES AND FOLDERS

dataverse/00-README.txt
This file.

dataverse/01_data.csv
Raw dataset.

dataverse/02_data_analysis.Rmd
Statistical analysis script for R and Rstudio.

dataverse/03_variables.txt
Names of the variables and description.

dataverse/04_codebook.html
Codebook with variables and frequencies.

=============
# PREREQUISITES

To recreate the analysis you need to
1. Install R, Rstudio and the pacman package 
2. unzip all the files and folders
3. run the RMD file using Rstudio and R

=============
# DATACODES
English	Description
country	country - Latvia/Lithuania
count	study unit - member of household
family_code	a code for each family (refers to one questionnaire)
nr_of_family_members	total number of people in the household
lives_in_specific	residency (city or region)
lives_in	type of living place - city/town/rural
age	age of the member of the household
toothpaste	toothpaste brand name
toothpaste_full_name	specific title of the toothpaste
f_concentration	fluoride concentration in the toothpaste

=============
# ABSTRACT
Background. Toothpaste with >1000 ppm fluoride effectively prevents tooth decay. In the European market, it is possible to find pastes with varying fluoride levels. We aim to quantify the use of toothpaste in Latvia and Lithuania according to the concentration of fluoride labelled in the toothpaste. Methods. After approval of the Riga Stradins University Ethics Committee, a cross-sectional survey-based study was carried out in December 2018 in nine schools all over Latvia. A previously validated questionnaire was used to collect demographic information and the type of toothpaste used by each family member. Descriptive statistics were obtained using program R and the tidyverse package. Results. A total of 307 children and their families participated. The response rate was 69.4%, and ten questionnaires were discarded for being incomplete. A total of 203 questionnaires gave information about 1016 family members (mean age 25.9 years, range 1-84). We registered 228 different kinds of toothpaste, of which 54 were without fluoride. In 11.8% of families, one toothpaste for all household members is used, but in 57.1% of families, special children toothpaste is chosen for children. 15.6% of people reported using toothpaste without fluoride, 15.1% with less than 1000ppm and 62% using fluoride over 1000ppm. The proportion of people who use fluoride-free toothpaste is greater in the adult age group (19%) and those, who use toothpaste with 550 ppm or less, greater in children aged 1-5 years (32%).  Conclusions. In 62% of Latvian families, toothpastes containing the optimal concentration of fluoride are used. This suggests that a significant percentage of families occupy toothpaste with little or no effectiveness against tooth decay. Efforts should, therefore, be made to communicate to patients about the correct use of this important preventive and therapeutic strategy to reduce dental caries.

Key Words: fluoride, fluoride toothpaste, dental public health, non-invasive caries treatment, survey research


=============
# SOFTWARE AND PACKAGES USED

> sessionInfo()
R version 4.1.2 (2021-11-01)
Platform: x86_64-pc-linux-gnu (64-bit)
Running under: Pop!_OS 22.04 LTS

Matrix products: default
BLAS:   /usr/lib/x86_64-linux-gnu/blas/libblas.so.3.10.0
LAPACK: /usr/lib/x86_64-linux-gnu/lapack/liblapack.so.3.10.0

locale:
 [1] LC_CTYPE=en_GB.UTF-8       LC_NUMERIC=C               LC_TIME=en_US.UTF-8        LC_COLLATE=en_GB.UTF-8     LC_MONETARY=en_US.UTF-8   
 [6] LC_MESSAGES=en_GB.UTF-8    LC_PAPER=en_US.UTF-8       LC_NAME=C                  LC_ADDRESS=C               LC_TELEPHONE=C            
[11] LC_MEASUREMENT=en_US.UTF-8 LC_IDENTIFICATION=C       

attached base packages:
[1] stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
 [1] viridis_0.6.2      viridisLite_0.4.1  leaflet_2.1.1      RColorBrewer_1.1-3 ggpubr_0.5.0       gtsummary_1.6.2    table1_1.4.2      
 [8] scales_1.2.1       MatchIt_4.5.0      janitor_2.1.0      here_1.0.1         kableExtra_1.3.4   forcats_0.5.2      stringr_1.4.1     
[15] dplyr_1.0.10       purrr_0.3.5        readr_2.1.3        tidyr_1.2.1        tibble_3.1.8       ggplot2_3.4.0      tidyverse_1.3.2   

loaded via a namespace (and not attached):
 [1] fs_1.5.2            lubridate_1.9.0     bit64_4.0.5         webshot_0.5.4       httr_1.4.4          rprojroot_2.0.3     bslib_0.4.1        
 [8] tools_4.1.2         backports_1.4.1     utf8_1.2.2          R6_2.5.1            DBI_1.1.3           colorspace_2.0-3    withr_2.5.0        
[15] tidyselect_1.2.0    gridExtra_2.3       curl_4.3.3          bit_4.0.5           compiler_4.1.2      cli_3.4.1           rvest_1.0.3        
[22] gt_0.8.0            pacman_0.5.1        xml2_1.3.3          sass_0.4.2          labeling_0.4.2      commonmark_1.8.1    systemfonts_1.0.4  
[29] digest_0.6.30       rmarkdown_2.18      svglite_2.1.0       pkgconfig_2.0.3     htmltools_0.5.3     highr_0.9           dbplyr_2.2.1       
[36] fastmap_1.1.0       htmlwidgets_1.5.4   rlang_1.0.6         readxl_1.4.1        rstudioapi_0.14     jquerylib_0.1.4     farver_2.1.1       
[43] generics_0.1.3      jsonlite_1.8.3      crosstalk_1.2.0     vroom_1.6.0         car_3.1-1           googlesheets4_1.0.1 magrittr_2.0.3     
[50] Formula_1.2-4       Rcpp_1.0.9          munsell_0.5.0       fansi_1.0.3         abind_1.4-5         lifecycle_1.0.3     stringi_1.7.8      
[57] snakecase_0.11.0    carData_3.0-5       grid_4.1.2          parallel_4.1.2      crayon_1.5.2        haven_2.5.1         hms_1.1.2          
[64] knitr_1.40          pillar_1.8.1        ggsignif_0.6.4      reprex_2.0.2        glue_1.6.2          evaluate_0.18       broom.helpers_1.9.0
[71] modelr_0.1.10       vctrs_0.5.1         tzdb_0.3.0          cellranger_1.1.0    gtable_0.3.1        assertthat_0.2.1    cachem_1.0.6       
[78] xfun_0.34           broom_1.0.1         rstatix_0.7.1       googledrive_2.0.0   gargle_1.2.1        timechange_0.1.1    ellipsis_0.3.2     
