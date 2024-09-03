## Analysis Overview
### Steps taken during the analysis
The synthetic CMS Home Health Agency data was uploaded into Google Colab. The data columns were printed and organized. 
Eight columns were selected to find each value's unique value count and frequency. 

### Selected Columns
- PRNCPAL_DGNS_CD: code Z733 
- ICD_DGNS_CD10: code G43719
- ICD_DGNS_CD5: code E669
- ICD_DGNS_CD14: code E8881
- ICD_DGNS_CD2: code M179
- ICD_DGNS_CD19: code R4689
- ICD_DGNS_CD8: code R52
- HCPCS_CD: code S9122

### Meaning of Each Code
- Z733: stress, not elsewhere classified 
- G43719: Chronic migraine without aura, intractable, without status migrainosus
- E669: Obesity, unspecified
- E8881: Metabolic syndrome and other insulin resistance
- M179: Osteoarthritis of knee, unspecified
- R4689: Other symptoms and signs involving appearance and behavior
- R52: Pain, unspecified
- S9122: Laceration with foreign body of toe with damage to nail


### Key Findings and Challenges 
The patient diagnosis code 'Z733' was generally the most common. Once I started analyzing the ICD diagnosis codes, I noticed more differences in the data.
The biggest challenge was that much of the data contained 'NaN' values, which appeared in at least two columns. I tried removing the 'NaN' values from the fourth column, 
which reduced the total unique count from 55 to 54. It seemed that 'NaN' values were not included in the frequency count for each code.
