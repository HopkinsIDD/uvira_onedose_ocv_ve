![image](https://github.com/HopkinsIDD/uvira_onedose_ocv_ve/assets/39589976/9ed66ac8-5f2c-43b3-969b-101832403b8e)

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
| ocv_2dose     |  string ('Two doses' or 'Not vaccinated') | classification of vaccination status by receipt of of two doses of kOCV     | 
| ocv_atleast_1dose | string ('At least one dose' or 'Not vaccinated')  | classification of vaccination status by receipt of at least one dose of kOCV | 
| ocv_all_dose  | string ('Two doses', 'One dose', 'Not vaccinated')| overall classification of the vaccination status | 
| vaccine_card | string ('Available', 'Unavailable') | availability of the vaccination card for those reporting to be vaccinated |
| ind_vacc_card | string ('yes', 'no') | availability of the vaccination card for those reporting to be vaccinated |

2. `df_period2.rds`

This date set includes all the variables available in 'df_period1.rds', with additional data on household characteristics.

| variable name | variable type | definition |
|---------------|---------------|------------|
| drinking_water_source  | string  ('Improved' or 'Unimproved') | drinking water source used by the participant, classified based on the JMP criteria| 
| educ  | string ('None or primary', 'Lower secondary', 'Upper secondary', or 'Bachelors or higher')  | level of education attainment|
| handwash_soapwater  | string ('No' or 'Yes') | availability of a handwashing facility with soap and water in the household|  
| hh_size | integer | number of people in the participant's household |
| n_hh_centered | decimal| household size centered to the mean |    
| occup | string ('No work', 'Preschool children', 'Students', 'Informal work', 'Salaried')| participant's occupation|
| toilet_shared |string ('Private' or 'Shared' | whether the participant used a toilet shared by multiple households compared with using a private toilet|
|toilet_type  | string ('Improved' or 'Unimproved') | type of sanitation facility, based on JMP classification   | 
|wealth_index | decimal | wealth index derived from principal component analysis of household assets and housing structure |
| wealth_index_centered | decimal | wealth index derived from principal component analysis of household assets, and centered to the mean|

   
3. `df_combined.rds`

The `df_combined.rds` data set contains the same variable as `df_period1.rds`.
