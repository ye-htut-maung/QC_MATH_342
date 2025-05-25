for the sale_price, for missingness, first you impute and then drop



note from Tao

# Packages/Libraries Setup
# Data Import
# Data Preparation
# Data Cleaning I (Errors, Duplicates, Outliers Handling)
# Data Manipulation (Featurization)
# Swift Data Exploration
# Linear Modeling
# Regression Tree Modeling
# Random Forest Modeling
# Performance Validation
# Report Goodness-of-fit Metrics in One Clear Table
# Shipping Final Model Trained On All Data


── Data Summary ────────────────────────
                           Values                      
Name                       Xy_without_useless_featur...
Number of rows             2230                        
Number of columns          32                          
Key                        NULL                        
_______________________                                
Column type frequency:                                 
  character                18                          
  numeric                  14                          
________________________                               
Group variables            None                        

── Variable type: character ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
   skim_variable                 n_missing complete_rate min max empty n_unique whitespace
 1 URL                                 758         0.660  73 105     0     1450          0
 2 cats_allowed                          0         1       1   3     0        3          0
 3 common_charges                     1684         0.245   3   7     0      258          0
 4 coop_condo                            0         1       5   5     0        2          0
 5 date_of_sale                       1702         0.237   8  10     0      222          0
 6 dining_room_type                    448         0.799   4  11     0        5          0
 7 dogs_allowed                          0         1       2   5     0        3          0
 8 fuel_type                           112         0.950   3   8     0        6          0
 9 full_address_or_zip_code              0         1       5  59     0     1177          0
10 garage_exists                      1826         0.181   1  11     0        6          0
11 kitchen_type                         16         0.993   4  19     0       13          0
12 maintenance_cost                    623         0.721   4   7     0      609          0
13 model_type                           40         0.982   1  40     0      875          0
14 parking_charges                    1671         0.251   2   4     0       89          0
15 sale_price                         1702         0.237   8   9     0      315          0
16 total_taxes                        1646         0.262   3   7     0      293          0
17 listing_price_to_nearest_1000       534         0.761   3   7     0      292          0
18 url                                1472         0.340  73 105     0      758          0

── Variable type: numeric ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
   skim_variable               n_missing complete_rate     mean      sd   p0  p25  p50  p75 p100 hist 
 1 MaxAssignments                    758        0.660     1       0        1    1    1    1    1 ▁▁▇▁▁
 2 AssignmentDurationInSeconds       758        0.660   900       0      900  900  900  900  900 ▁▁▇▁▁
 3 AutoApprovalDelayInSeconds        758        0.660    60       0       60   60   60   60   60 ▁▁▇▁▁
 4 WorkTimeInSeconds                 758        0.660   162.    112.      22   89  127  197  815 ▇▂▁▁▁
 5 approx_year_built                  40        0.982  1963.     21.1   1893 1950 1958 1970 2017 ▁▂▇▂▂
 6 community_district_num             19        0.991    26.3     2.95     3   25   26   28   32 ▁▁▁▇▇
 7 num_bedrooms                      115        0.948     1.65    0.744    0    1    2    2    6 ▇▇▂▁▁
 8 num_floors_in_building            650        0.709     7.79    7.52     1    3    6    7   34 ▇▁▁▁▁
 9 num_full_bathrooms                  0        1         1.23    0.445    1    1    1    1    3 ▇▁▂▁▁
10 num_half_bathrooms               2058        0.0771    0.953   0.302    0    1    1    1    2 ▁▁▇▁▁
11 num_total_rooms                     2        0.999     4.14    1.35     0    3    4    5   14 ▁▇▂▁▁
12 pct_tax_deductibl                1754        0.213    45.4     6.95    20   40   50   50   75 ▁▅▇▁▁
13 sq_footage                       1210        0.457   955.    381.     100  743  881 1100 6215 ▇▁▁▁▁
14 walk_score                          0        1        83.9    14.7      7   77   89   95   99 ▁▁▁▂▇




get zip code from URL and full_address_or_zip_code
drop model or get 10 factors

then imputation



