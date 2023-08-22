# MSKCC-Oncokb-Actionability-
- Scripts to make Oncokb Actionability Figure
- Modified the original code from https://github.com/sas1531/Actionability-MSKCC-OncoKB to suit GENIE data files.

# Usage:

**action_levels_barplot_fun: Creates actionability barplot displaying the highest level of evidence for each sample across all cancer types.**

action_levels_barplot_fun(cna_df, mut_df, fus_df, clin_df, data_freeze,
                          group_col = "ONCOTREE_CODE",
                          status = c("somatic", "germline", "both"),
                          consent_col = "Consent") 

**action_main_fun: Creates main tile plot displaying the frequency of highest level of evidence of a specific alteration across all cancer types that have a minimum aletration frequency of 1%.**

action_main_fun(cna_df, mut_df, fus_df, clin_df, data_freeze,
                path_df, tsg_list, fusion_list, gene_order,
                prop_level_df = "./actionability_levels_barplot_table.txt",
                group_col = "ONCOTREE_CODE",
                status = c("somatic"),
                consent_col = "Consent"
                alt_min = 1)

                
