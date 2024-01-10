Welcome to the code and data repository for "Effectiveness of one dose of killed oral cholera vaccine in an
endemic community in the Democratic Republic of the
Congo: a matched case-control study" by Malembaka et al. 

## Data 

We provide three data sets from this study to reproduce analyses. One file from study period 1 (`data/df_period1.rds`), one from study period 2 (`data/df_period1.rds`) and one of the combined data across periods (`data/df_combined.rds`). 

1. `df_period1.rds`
   
| variable name | variable type | definition |
|---------------|---------------|------------|
| record_id     | string        | unique record id | 
| id_case       | string        | unique id of matched case (equal to record_id when this is a case|
| case_status   | string ('case' or 'control') | indicates whether case or control|  
| case_control  | binary        | 0 if control, 1 if case |
| age_vacc      | decimal       | age at vaccination in years|
| age_group_vacc | string       | age group at vaccination in years|
| cat_sex        |  string            |   sex of the participant               | 
| ocv_single_dose | string ('Single dose' or 'Not vaccinated')     | classification of vaccination status for main analysis|
| ocv_2dose     |  string ('Two doses' or 'Not vaccinated' | classification of vaccination status by receipt of of two doses of kOCV     | 
| ocv_atleast_1dose | string ('At least one dose' or 'Not vaccinated'  | classification of vaccination status by receipt of at least one dose of kOCV | 
| ocv_all_dose  | string ('Two doses', 'One dose', 'Not vaccinated')| overall classification of the vaccination status | 
| vaccine_card | string ('Available', 'Unavailable' | availability of the vaccination card for those reporting to be vaccinated |
| ind_vacc_card | string ('yes', 'no' | availability of the vaccination card for those reporting to be vaccinated |

2. `df_period2.rds`
   
3. `df_combined.rds` 
