## DHS Data Access Instructions

Note: These instructions were developed for students in a course at Middlebury.  There is no guarantee that the DHS program will continue to approve projects for replication of this study in the future.

1. Go to [https://dhsprogram.com/Data/](https://dhsprogram.com/Data/)
1. Create an account with your college e-mail address
2. Within the Datasets menu, [Create a new project](https://dhsprogram.com/data/dataset_admin/index.cfm?action=createproject)
1. Enter the following information:
**Project Title:** Reproducing a Vulnerability Model of Malawi
**Description of Study:** The purpose of this study is to reproduce the methods of a published research article: Malcomb, D. W., E. A. Weaver, and A. R. Krakowka. 2014. Vulnerability modeling for sub-Saharan Africa: An operationalized approach in Malawi. Applied Geography 48:17–30. http://dx.doi.org/10.1016/j.apgeog.2014.01.004. The authors of this paper used geocoded DHS surveys for Malawi in 2004 and 2010, in combination with FEWSnet livelihood data and UNEP flood and drought risk data. Following the author's methodology, we plan to download the data using the rdhs package for R and aggregate the data at Malawi's 2nd administrative level: districts. We will be working with a GitHub repository that stores the raw data locally in a directory ignored by the .gitignore file, and only moves the data into a shared and version-controlled directory once it has been aggregated to the District level. This will ensure that the privacy of survey respondents and requirements of data partners are protected, because all of the data will be aggregated into district polygons, as already shown and published in Malcomb et al (2014). The raw individual-level data will be deleted once the analysis is complete by May 31, 2021.
1. Choose Region: Sub-Saharan Africa
1. Click **Show GPS Datasets** at the top-left of the country tables
1. Check **Survey** and **GPS** data for **Malawi**
1. Save selection
1. Read and agree to the conditions of use for the DHS Program datasets and save these conditions for your metadata records.
1. Enter a **Justification for using DHS Program Geographic Datasets:** The research aim is to reproduce Malcomb et al (2014) in which GPS Datasets are used to spatially join DHS Survey data to Malawi's Districts for the purpose of sub-national climate change vulnerability mapping. Therefore, the research will not be reproducible without the geographic datasets.

## Geographic Structure of DHS Surveys

See maps and boundaries guiding the DHS Surveys for Malawi here: [http://spatialdata.dhsprogram.com/boundaries/#view=table&countryId=MW](http://spatialdata.dhsprogram.com/boundaries/#view=table&countryId=MW)

And the boundaries for the 2010 Level 2 survey here: [http://spatialdata.dhsprogram.com/boundaries/#view=map&countryId=MW&surveyId=333&level=2](http://spatialdata.dhsprogram.com/boundaries/#view=map&countryId=MW&surveyId=333&level=2)

And Summary of the 2010 Survey here: [https://www.dhsprogram.com/methodology/survey/survey-display-333.cfm](https://www.dhsprogram.com/methodology/survey/survey-display-333.cfm)

## Extract of the SPSS Data Structure for 2010

### VARIABLE LABELS
   HHID     "Case Identification"
  /HVIDX    "Line number"
  /HV000    "Country code and phase"
  /HV001    "Cluster number"
  /HV002    "Household number"
  /HV003    "Respondent's line number"
  /HV004    "Ultimate area unit"
  /HV005    "Sample weight"
  /HV006    "Month of interview"
  /HV007    "Year of interview"
  /HV008    "Date of interview (CMC)"
  /HV009    "Number of household members"
  /HV010    "Number of eligible women in HH"
  /HV011    "Number of eligible men in HH"
  /HV012    "Number of de jure members"
  /HV013    "Number of de facto members"
  /HV014    "Number of children 5 and under"
  /HV015    "Result of household interview"
  /HV016    "Day of interview"
  /HV017    "Number of visits"
  /HV018    "Interviewer identification"
  /HV019    "Keyer identification"
  /HV020    "Ever-married sample"
  /HV021    "Primary sampling unit"
  /HV022    "Sample stratum number"
  /HV023    "Sample domain"
  /HV024    "Region"
  /HV025    "Type of place of residence"
  /HV026    "Place of residence"
  /HV027    "Selection for male/husb. int."
  /HV028    "Sample weight for male subsamp"
  /HV030    "Field supervisor"
  /HV031    "Field editor"
  /HV032    "Office editor"
  /HV033    "NA - Ultimate area selection prob."
  /HV035    "Number of eligible children for height & weight"
  /HV040    "Cluster altitude in meters"
  /HV041    "Total adults measured"
  /HV042    "Selection for hemoglobin"
  /HV043    "NA - Selection for women's status module"
  /HV044    "Selection for domestic violence module"
  /HV201    "Source of drinking water"
  /HV202    "NA - Source of non-drinking water"
  /HV204    "Time to get to water source"
  /HV205    "Type of toilet facility"
  /HV206    "Has electricity"
  /HV207    "Has radio"
  /HV208    "Has television"
  /HV209    "Has refrigerator"
  /HV210    "Has bicycle"
  /HV211    "Has motorcycle/scooter"
  /HV212    "Has car/truck"
  /HV213    "Main floor material"
  /HV214    "Main wall material"
  /HV215    "Main roof material"
  /HV216    "Rooms used for sleeping"
  /HV217    "Relationship structure"
  /HV218    "Line number of head of househ."
  /HV219    "Sex of head of household"
  /HV220    "Age of head of household"
  /HV221    "Has a landline telephone"
  /HV225    "Share toilet with other households"
  /HV226    "Type of cooking fuel"
  /HV227    "Have bednet for sleeping"
  /HV228    "Children under 5 slept under bednet last night"
  /HV234    "Test salt for Iodine"
  /HV235    "Location of source for water"
  /HV236    "Person fetching water"
  /HV237    "Anything done to water to make safe to drink"
  /HV237A   "Water usually treated by: boil"
  /HV237B   "Water usually treated by: add bleach/chlorine"
  /HV237C   "Water usually treated by: strain through a cloth"
  /HV237D   "Water usually treated by: use water filter"
  /HV237E   "Water usually treated by: solar disinfection"
  /HV237F   "Water usually treated by: let it stand and settle"
  /HV237G   "NA - Water usually treated by: CS"
  /HV237H   "NA - Water usually treated by: CS"
  /HV237I   "NA - Water usually treated by: CS"
  /HV237J   "NA - Water usually treated by: CS"
  /HV237K   "NA - Water usually treated by: CS"
  /HV237X   "Water usually treated by: other"
  /HV237Z   "Water usually treated by: don't know"
  /HV238    "Number of households sharing toilet"
  /HV239    "Food cooked on stove or open fire"
  /HV240    "Household has a chimney, hood or neither"
  /HV241    "Food cooked in the house / in separate building / outdoors"
  /HV242    "Household has separate room used as kitchen"
  /HV243A   "Has a mobile telephone"
  /HV243B   "Has a watch"
  /HV243C   "Has an animal-drawn cart"
  /HV243D   "NA - Has a boat with a motor"
  /HV244    "Own land usable for agriculture"
  /HV245    "Hectares for agricultural land"
  /HV246    "Livestock, herds or farm animals"
  /HV246A   "Cattle own"
  /HV246B   "NA - Cows, bulls own"
  /HV246C   "NA - Horses, donkeys, mules own"
  /HV246D   "Goats own"
  /HV246E   "Sheep own"
  /HV246F   "Poultry own"
  /HV246G   "Pigs own"
  /HV246H   "NA - CS own"
  /HV246I   "NA - CS own"
  /HV246J   "NA - CS own"
  /HV246K   "Other own"
  /HV247    "Owns a bank account"
  /HV248    "Number of sick people 18-59"
  /HV249    "Member of the HH died last 12 months"
  /HV250    "Number of members who died last 12 months"
  /HV251    "Number of orphans and vulnerable children"
  /HV270    "Wealth index"
  /HV271    "Wealth index factor score (5 decimals)"
  /HML1     "Number of mosquito nets"
  /HML1A    "Number of mosquito nets with specific information"
  /HML2     "Number of children under bednet previous night"
  /SHDIST   "District"
  /SHLQUEST "Language of Questionnaire"
  /SHLRESP  "Native language of respondent"
  /SHLINT   "Language of interview"
  /SHLTRANS "Translator used"
  /SHLRESO  "Other: Native language of respondent"
  /SH111A2  "Koloboyi"
  /SH111B   "Paraffin lamp other than koloboyi"
  /SH111G   "Bed with mattress"
  /SH111H   "Sofa set"
  /SH111I   "Table and chairs"
  /SH123    "Amount of agricultural land owned"
  /SH126A   "Walls sprayed for mosquitos in past 12 months"
  /SH126B   "Months ago house was sprayed"
  /SH126C   "Those who sprayed"
  /SH138    "Color of net preferred"
  /SH139    "Shape of net preferred"
  /SH139A   "Shown place for washing hands"
  /SH139B   "Water available at location for hand washing"
  /SH139CA  "Soap available at location for hand washing"
  /SH139CB  "Soap available at location for hand washing"
  /SH139CY  "Soap available at location for hand washing"
  /SH140    "Test salt for Iodine"
  /HV101    "Relationship to head"
  /HV102    "Usual resident"
  /HV103    "Slept last night"
  /HV104    "Sex of household member"
  /HV105    "Age of household members"
  /HV106    "Highest educational level"
  /HV107    "Highest year of education"
  /HV108    "Education in single years"
  /HV109    "Educational attainment"
  /HV110    "NA - Member still in school"
  /HV111    "Mother alive"
  /HV112    "Mother's line number"
  /HV113    "Father alive"
  /HV114    "Father's line number"
  /HV115    "NA - Current marital status"
  /HV116    "Currently, formerly, never m."
  /HV117    "Eligibility for female interview"
  /HV118    "Eligibility for male interview"
  /HV120    "Children eligibility for height/weight and hemoglobin"
  /HV121    "Member attended school during current school year"
  /HV122    "Educational level during current school year"
  /HV123    "Grade of education during current school year"
  /HV124    "Education in single years - current school year"
  /HV125    "Member attended school during previous school year"
  /HV126    "Educational level during previous school year"
  /HV127    "Grade of education during previous school year"
  /HV128    "Education in single years - previous school year"
  /HV129    "School attendance status"
  /HV130    "Member has been very sick for 3+ months last year"
  /HV131    "Mother has been very sick for 3+ months last year"
  /HV132    "Father has been very sick for 3+ months last year"
  /HV133    "Mother/father dead or been very sick for 3+ months"
  /HV134    "NA - Both parents alive"
  /HV135    "NA - Has brothers/sisters under 18 of the same father and mother"
  /HV136    "NA - Brothers/sisters under 18 that don't live in household"
  /HV137    "Member has a blanket"
  /HV138    "Member has a pair of shoes"
  /HV139    "Member has 2+ sets of clothes"
  /HV140    "NA - Member has a birth certificate"
  /IDXH4    "Index to household schedule"
  /SH08     "Marital status"
  /SH24A    "Level of education attended"
  /SH26A    "Level of education attending"
  /SH28A    "Level of education last year"
  /SH32     "Meals eaten yesterday"
  /HA0      "Index to household schedule"
  /HA1      "Women's age in years"
  /HA2      "Respondent's weight (kilos-1d)"
  /HA3      "Respondent's height (cms-1d)"
  /HA4      "Ht/A Percentile (resp.)"
  /HA5      "Ht/A Standard deviations (resp"
  /HA6      "Ht/A Percent ref. median (resp"
  /HA11     "Wt/Ht Std deviations(resp) DHS"
  /HA12     "Wt/Ht Percent ref. median (DHS"
  /HA12A    "Wt/Ht Percent ref. median (Fog"
  /HA12B    "Wt/Ht Percent ref. median (WHO"
  /HA13     "Result of measurement of resp."
  /HA32     "Date of birth (cmc)"
  /HA33     "Completeness of information"
  /HA35     "Smoking"
  /HA40     "Body mass index for respondent"
  /HA41     "Rohrer's index for respondent"
  /HA50     "Under age 18"
  /HA51     "Line no. of parent/caretaker"
  /HA52     "Read consent statement"
  /HA53     "Hemoglobin level (g/dl - 1 decimal)"
  /HA54     "Currently pregnant"
  /HA55     "Result of measuring (Hemoglobin)"
  /HA56     "Hemoglobin level adjusted by altitude (g/dl - 1 decimal)"
  /HA57     "Anemia level"
  /HA58     "NA - Agrees to referral"
  /HA60     "Marital status"
  /HA61     "Read consent statement (HIV)"
  /HA62     "Blood sample ID number"
  /HA63     "Result of measuring (HIV)"
  /HA64     "Consent for additional tests"
  /HA65     "Result of woman individual interview"
  /HA66     "Woman's highest educational level"
  /HA67     "Woman's highest year of education"
  /HA68     "Highest educational level (CS for preliminary & final report)"
  /HA69     "HIV weight (6 decimals)"
  /SH517    "Weight in kilograms"
  /SH518    "Height in centimeters"
  /SH523B   "Read parent consent statement (Anemia)"
  /SH523D   "Read respondent consent statement (Anemia)"
  /SH525B   "Read parent consent statement (HIV)"
  /SH525C   "HIV status disclosure"
  /SH525F   "Read respondent consent statement (HIV)"
  /SH525G   "Age/married check"
  /SH525J   "Read parent consent statement (Additional tests)"
  /SH525L   "Read respondent consent statement (Additional tests)"
  /SH527    "Hemoglobin level (g/dl)"
  /HC0      "Index to household schedule"
  /HC1      "Age in months"
  /HC2      "Weight in kilograms (1 dec.)"
  /HC3      "Height in centimeters (1 dec.)"
  /HC4      "Ht/A Percentile"
  /HC5      "Ht/A Standard deviations"
  /HC6      "Ht/A Percent of ref. median"
  /HC7      "Wt/A Percentile"
  /HC8      "Wt/A Standard deviations"
  /HC9      "Wt/A Percent of ref. median"
  /HC10     "Wt/Ht Percentile"
  /HC11     "Wt/Ht Standard deviations"
  /HC12     "Wt/Ht Percent of ref. median"
  /HC13     "Result of measurement"
  /HC15     "Height: lying or standing"
  /HC16     "Day of birth of child"
  /HC17     "Date measured (day)"
  /HC18     "Date measured (month)"
  /HC19     "Date measured (year)"
  /HC27     "Sex"
  /HC30     "Month of birth of child"
  /HC31     "Year of birth of child"
  /HC32     "Date of birth (cmc)"
  /HC33     "Completeness of information"
  /HC51     "Line no. of parent/caretaker"
  /HC52     "Read consent statement"
  /HC53     "Hemoglobin level (g/dl - 1 decimal)"
  /HC55     "Result of measuring (Hemoglobin)"
  /HC56     "Hemoglobin level adjusted by altitude (g/dl - 1 decimal)"
  /HC57     "Anemia level"
  /HC58     "NA - Agrees to referral"
  /HC60     "Mother's line number from woman's questionnaire"
  /HC61     "Mother's highest educational level"
  /HC62     "Mother's highest year of education"
  /HC63     "Preceding birth interval"
  /HC64     "Birth order number"
  /HC68     "Highest educational level (CS for preliminary & final report)"
  /HC70     "Ht/A Standard deviations (according to WHO)"
  /HC71     "Wt/A Standard deviations (according to WHO)"
  /HC72     "Wt/Ht Standard deviations (according to WHO)"
  /HC73     "BMI Standard deviations (according to WHO)"
  /SH505    "Weight in kilograms"
  /SH506    "Height in centimeters"
  /SH507    "Height: lying or standing"
  /SH512    "Hemoglobin level (g/dl)"
  /HB0      "Index to household schedule"
  /HB1      "Men's age in years"
  /HB2      "NA - Respondent's weight (kilos-1d)"
  /HB3      "NA - Respondent's height (cms-1d)"
  /HB4      "NA - Ht/A Percentile (resp.)"
  /HB5      "NA - Ht/A Standard deviations (resp"
  /HB6      "NA - Ht/A Percent ref. median (resp"
  /HB11     "NA - Wt/Ht Std deviations(resp) DHS"
  /HB12     "NA - Wt/Ht Percent ref. median (DHS"
  /HB12A    "NA - Wt/Ht Percent ref. median (Fog"
  /HB12B    "NA - Wt/Ht Percent ref. median (WHO"
  /HB13     "NA - Result of measurement of resp."
  /HB32     "Date of birth (cmc)"
  /HB33     "Completeness of information"
  /HB35     "Smoking"
  /HB40     "NA - Body mass index for respondent"
  /HB41     "NA - Rohrer's index for respondent"
  /HB50     "Under age 18"
  /HB51     "Line no. of parent/caretaker"
  /HB52     "NA - Read consent statement"
  /HB53     "NA - Hemoglobin level (g/dl - 1 decimal)"
  /HB55     "NA - Result of measuring (Hemoglobin)"
  /HB56     "NA - Hemoglobin level adjusted by altitude (g/dl - 1 decimal)"
  /HB57     "NA - Anemia level"
  /HB58     "NA - Agrees to referral"
  /HB60     "Marital status"
  /HB61     "Read consent statement (HIV)"
  /HB62     "Blood sample ID number"
  /HB63     "Result of measuring (HIV)"
  /HB64     "Consent for additional tests"
  /HB65     "Result of man individual interview"
  /HB66     "Man's highest educational level"
  /HB67     "Man's highest year of education"
  /HB68     "Highest educational level (CS for preliminary & final report)"
  /HB69     "HIV weight (6 decimals)"
  /SH533    "Respondent present"
  /SH540B   "Read parent consent statement (HIV)"
  /SH540C   "HIV status disclosure"
  /SH540F   "Read respondent consent statement (HIV)"
  /SH540G   "Under age 18"
  /SH540J   "Read parent consent statement (Additional tests)"
  /SH540L   "Read respondent consent statement (Additional tests)"
  /HMLIDX   "Net number"
  /HML3     "Net observed"
  /HML4     "Months ago obtained mosquito net"
  /HML5     "NA - Was net treated with insecticide when bought"
  /HML6     "Mosquito net treated with insecticide"
  /HML7     "Brand of bednet"
  /HML8     "Bednet treated since receiving"
  /HML9     "Months ago re-treated"
  /HML10    "ITN net"
  /HML11    "Number of persons who slept under this net"
  /HML21    "Did someone sleep under bednet last night"
  /HMLA     "Person who slept in mosquito net"
  /HMLB     "Person who slept in mosquito net"
  /HMLC     "Person who slept in mosquito net"
  /HMLD     "Person who slept in mosquito net"
  /HMLE     "NA - Person who slept in mosquito net"
  /SH129A   "Net has holes"
  /SH129B   "Color of net"
  /SH129C   "Shape of net"
  /SH130C   "Net came with treatment kit"
  /HMHIDX   "Index to household schedule"
  /HML12    "Type of bednet(s) person slept under last night"
  /HML13    "1st net number for net person slept under last night"
  /HML14    "2nd net number for net person slept under last night"
  /HML15    "NA - 3rd net number for net person slept under last night"
  /HML16    "Corrected age from individual questionnaire"
  /HML17    "Flag for HV105 age from individual file"
  /HML18    "Pregnancy from individual questionnaire"
  /HML19    "Person sleep under an ever treated bednet"
  /HSKIDX   "Index to household schedule"
  /HS100    "Free medical support last 12 months"
  /HS101    "Medical support at least once a month"
  /HS102    "Free emotional support last 12 months"
  /HS103    "Emotional support last 30 days"
  /HS104    "Free material support last 12 months"
  /HS105    "Material support last 30 days"
  /HS106    "Free social support last 12 months"
  /HS107    "Social support last 30 days"
  /HS108    "NA - Pain last 30 days"
  /HS109    "NA - Able to reduce the pain"
  /HS110    "NA - Nausea last 30 days"
  /HS111    "NA - Able to reduce the nausea"
  /HOVIDX   "Index to household schedule"
  /HO100    "Age of child"
  /HO101    "Free medical support last 12 months"
  /HO102    "Free emotional support last 12 months"
  /HO103    "Emotional support last 3 months"
  /HO104    "Free material support last 12 months"
  /HO105    "Material support last 3 months"
  /HO106    "Free social support last 12 months"
  /HO107    "Social support last 3 months"
  /HO108    "Free support for schooling"
  /SH416AA  "Assistance received for schooling"
  /SH416AB  "Assistance received for schooling"
  /SH416AC  "Assistance received for schooling"
  /SH416AD  "Assistance received for schooling"
  /SH416AX  "Assistance received for schooling"

### MISSING VALUE
   HV026    (9)
  /HV040    (9999)
  /HV201    (99)
  /HV202    (99)
  /HV204    (999)
  /HV205    (99)
  /HV206    (9)
  /HV207    (9)
  /HV208    (9)
  /HV209    (9)
  /HV210    (9)
  /HV211    (9)
  /HV212    (9)
  /HV213    (99)
  /HV214    (99)
  /HV215    (99)
  /HV216    (99)
  /HV219    (9)
  /HV220    (99)
  /HV221    (9)
  /HV225    (9)
  /HV226    (99)
  /HV227    (9)
  /HV228    (9)
  /HV234    (999)
  /HV235    (9)
  /HV236    (9)
  /HV237    (9)
  /HV237A   (9)
  /HV237B   (9)
  /HV237C   (9)
  /HV237D   (9)
  /HV237E   (9)
  /HV237F   (9)
  /HV237G   (9)
  /HV237H   (9)
  /HV237I   (9)
  /HV237J   (9)
  /HV237K   (9)
  /HV237X   (9)
  /HV237Z   (9)
  /HV238    (99)
  /HV239    (9)
  /HV240    (9)
  /HV241    (9)
  /HV242    (9)
  /HV243A   (9)
  /HV243B   (9)
  /HV243C   (9)
  /HV243D   (9)
  /HV244    (9)
  /HV245    (99)
  /HV246    (9)
  /HV246A   (99)
  /HV246B   (99)
  /HV246C   (99)
  /HV246D   (99)
  /HV246E   (99)
  /HV246F   (99)
  /HV246G   (99)
  /HV246H   (99)
  /HV246I   (99)
  /HV246J   (99)
  /HV246K   (99)
  /HV247    (9)
  /HV250    (99)
  /HML1     (99)
  /HML2     (99)
  /SHLQUEST (9)
  /SHLRESP  (9)
  /SHLINT   (9)
  /SHLTRANS (9)
  /SH111A2  (9)
  /SH111B   (9)
  /SH111G   (9)
  /SH111H   (9)
  /SH111I   (9)
  /SH123    (1000)
  /SH126A   (9)
  /SH126B   (99)
  /SH126C   (9)
  /SH138    (9)
  /SH139    (9)
  /SH139A   (9)
  /SH139B   (9)
  /SH139CA  (9)
  /SH139CB  (9)
  /SH139CY  (9)
  /SH140    (9)
  /HV101    (99)
  /HV102    (9)
  /HV103    (9)
  /HV104    (9)
  /HV105    (99)
  /HV106    (9)
  /HV107    (99)
  /HV108    (99)
  /HV109    (9)
  /HV110    (9)
  /HV111    (9)
  /HV112    (99)
  /HV113    (9)
  /HV114    (99)
  /HV115    (9)
  /HV116    (9)
  /HV121    (9)
  /HV122    (9)
  /HV123    (99)
  /HV124    (99)
  /HV125    (9)
  /HV126    (9)
  /HV127    (99)
  /HV128    (99)
  /HV129    (9)
  /HV130    (9)
  /HV131    (9)
  /HV132    (9)
  /HV133    (9)
  /HV134    (9)
  /HV135    (9)
  /HV136    (9)
  /HV137    (9)
  /HV138    (9)
  /HV139    (9)
  /HV140    (9)
  /SH08     (9)
  /SH24A    (9)
  /SH26A    (9)
  /SH28A    (9)
  /HA2      (9999)
  /HA3      (9999)
  /HA4      (9999)
  /HA5      (9999)
  /HA6      (99999)
  /HA11     (9999)
  /HA12     (99999)
  /HA12A    (99999)
  /HA12B    (99999)
  /HA13     (9)
  /HA35     (99)
  /HA40     (9999)
  /HA41     (9999)
  /HA50     (9)
  /HA52     (9)
  /HA53     (999)
  /HA54     (9)
  /HA55     (9)
  /HA56     (999)
  /HA57     (9)
  /HA58     (9)
  /HA61     (9)
  /HA63     (9)
  /HA64     (9)
  /HA66     (9)
  /HA67     (99)
  /HA68     (9)
  /SH523B   (9)
  /SH523D   (9)
  /SH525B   (9)
  /SH525C   (9)
  /SH525F   (9)
  /SH525G   (9)
  /SH525J   (9)
  /SH525L   (9)
  /SH527    (100)
  /HC2      (9999)
  /HC3      (9999)
  /HC4      (9999)
  /HC5      (9999)
  /HC6      (99999)
  /HC7      (9999)
  /HC8      (9999)
  /HC9      (99999)
  /HC10     (9999)
  /HC11     (9999)
  /HC12     (99999)
  /HC13     (9)
  /HC15     (9)
  /HC16     (99)
  /HC27     (9)
  /HC30     (99)
  /HC31     (9999)
  /HC52     (9)
  /HC53     (999)
  /HC55     (9)
  /HC56     (999)
  /HC57     (9)
  /HC58     (9)
  /HC61     (9)
  /HC62     (99)
  /HC63     (999)
  /HC64     (99)
  /HC68     (9)
  /HC70     (9999)
  /HC71     (9999)
  /HC72     (9999)
  /HC73     (9999)
  /SH505    (100)
  /SH506    (1000)
  /SH507    (9)
  /SH512    (100)
  /HB2      (9999)
  /HB3      (9999)
  /HB4      (9999)
  /HB5      (9999)
  /HB6      (99999)
  /HB11     (9999)
  /HB12     (99999)
  /HB12A    (99999)
  /HB12B    (99999)
  /HB13     (9)
  /HB35     (99)
  /HB40     (9999)
  /HB41     (9999)
  /HB50     (9)
  /HB52     (9)
  /HB53     (999)
  /HB55     (9)
  /HB56     (999)
  /HB57     (9)
  /HB58     (9)
  /HB61     (9)
  /HB63     (9)
  /HB64     (9)
  /HB66     (9)
  /HB67     (99)
  /HB68     (9)
  /SH540B   (9)
  /SH540C   (9)
  /SH540F   (9)
  /SH540G   (9)
  /SH540J   (9)
  /SH540L   (9)
  /HML3     (9)
  /HML4     (99)
  /HML5     (9)
  /HML6     (9)
  /HML7     (99)
  /HML8     (9)
  /HML9     (99)
  /HML10    (9)
  /HML11    (9)
  /HML21    (9)
  /HMLA     (99)
  /HMLB     (99)
  /HMLC     (99)
  /SH129A   (9)
  /SH129B   (9)
  /SH129C   (9)
  /SH130C   (9)
  /HML12    (9)
  /HML16    (99)
  /HML18    (9)
  /HS100    (9)
  /HS101    (9)
  /HS102    (9)
  /HS103    (9)
  /HS104    (9)
  /HS105    (9)
  /HS106    (9)
  /HS107    (9)
  /HS108    (9)
  /HS109    (9)
  /HS110    (9)
  /HS111    (9)
  /HO100    (99)
  /HO101    (9)
  /HO102    (9)
  /HO103    (9)
  /HO104    (9)
  /HO105    (9)
  /HO106    (9)
  /HO107    (9)
  /HO108    (9)
  /SH416AA  (9)
  /SH416AB  (9)
  /SH416AC  (9)
  /SH416AD  (9)
  /SH416AX  (9)

### VALUE LABELS
   HV003   
      0 "Incomplete interview"
  /HV015   
      1 "Completed"
      2 "HH present, no resp"
      3 "HH absent"
      4 "Postponed"
      5 "Refused"
      6 "Dwelling vacant"
      7 "Dwelling destroyed"
      8 "Dwelling not found"
      9 "Other"
  /HV020   
      0 "All woman sample"
      1 "Ever married sample"
  /HV023   
      1 "Northern"
      2 "Central"
      3 "Southern"
  /HV024   
      1 "Northern"
      2 "Central"
      3 "Southern"
  /HV025   
      1 "Urban"
      2 "Rural"
  /HV026   
      0 "Capital"
      1 "Major city"
      2 "Town"
      3 "Rural"
  /HV027   
      0 "Not selected"
      1 "Men's survey"
      2 "Husband's survey"
  /HV042   
      0 "Not selected"
      1 "Selected"
  /HV043   
      0 "Household not selected"
      1 "Household selected"
  /HV044   
      0 "Household not selected"
      1 "Household selected"
  /HV201   
     10 "PIPED WATER"
     11 "Piped into dwelling"
     12 "Piped to yard/plot"
     13 "Public tap/standpipe"
     20 "TUBE WELL WATER"
     21 "Tube well or borehole"
     30 "DUG WELL (OPEN/PROTECTED)"
     31 "Protected well"
     32 "Unprotected well"
     40 "SURFACE WATER"
     41 "Protected spring"
     42 "Unprotected spring"
     43 "River/dam/lake/ponds/stream/canal/irirgation channel"
     51 "Rainwater"
     61 "Tanker truck"
     62 "Cart with small tank"
     71 "Bottled water"
     96 "Other"
  /HV202   
     10 "PIPED WATER"
     11 "Piped into dwelling"
     12 "Piped to yard/plot"
     13 "Public tap/standpipe"
     20 "TUBE WELL WATER"
     21 "Tube well or borehole"
     30 "DUG WELL (OPEN/PROTECTED)"
     31 "Protected well"
     32 "Unprotected well"
     40 "SURFACE WATER"
     41 "Protected spring"
     42 "Unprotected spring"
     43 "River/dam/lake/ponds/stream/canal/irirgation channel"
     51 "Rainwater"
     61 "Tanker truck"
     62 "Cart with small tank"
     71 "Bottled water"
     96 "Other"
  /HV204   
    996 "On premises"
    998 "Don't know"
  /HV205   
     10 "FLUSH TOILET"
     11 "Flush toilet"
     20 "PIT TOILET LATRINE"
     21 "Pit latrine - ventilated improved pit (VIP)"
     22 "Pit latrine - with slab"
     23 "Pit latrine - without slab / open pit"
     30 "NO FACILITY"
     31 "No facility/bush/field"
     41 "Composting toilet"
     42 "Bucket toilet"
     43 "Hanging toilet/latrine"
     96 "OTHER"
  /HV206   
      0 "No"
      1 "Yes"
  /HV207   
      0 "No"
      1 "Yes"
  /HV208   
      0 "No"
      1 "Yes"
  /HV209   
      0 "No"
      1 "Yes"
  /HV210   
      0 "No"
      1 "Yes"
  /HV211   
      0 "No"
      1 "Yes"
  /HV212   
      0 "No"
      1 "Yes"
  /HV213   
     10 "NATURAL"
     11 "Earth, sand"
     12 "Dung"
     20 "RUDIMENTARY"
     21 "Wood planks"
     22 "Palm, bamboo"
     23 "Broken bricks"
     30 "FINISHED"
     31 "Parquet, polished wood"
     32 "Vinyl, asphalt strips"
     33 "Ceramic tiles"
     34 "Cement"
     35 "Carpet"
     96 "OTHER"
  /HV214   
     10 "NATURAL"
     11 "No walls"
     12 "Cane / palm / trunks"
     13 "Dirt"
     20 "RUDIMENTARY"
     21 "Bamboo / tree trunk with mud"
     22 "Stone with mud"
     23 "Uncovered adobe"
     24 "Plywood"
     25 "Cardboard"
     26 "Reused wood"
     30 "FINISHED"
     31 "Cement"
     32 "Stone with lime / cement"
     33 "Burnt bricks"
     34 "Unburnt bricks"
     35 "Cement blocks"
     36 "Wood planks/Shingles"
     96 "OTHER"
  /HV215   
     10 "NATURAL"
     11 "No roof"
     12 "Thatch / palm leaf"
     13 "SOD"
     20 "RUDIMENTARY"
     21 "Rustic mat"
     22 "Palm / bamboo / grass"
     23 "Wood planks"
     24 "Cardboard"
     30 "FINISHED"
     31 "Iron sheets"
     32 "Wood"
     33 "Calamine / cement fiber"
     34 "Ceramic tiles"
     35 "Cement"
     36 "Roofing shingles"
     96 "OTHER"
  /HV217   
      0 "No adults"
      1 "One adult"
      2 "Two adults, opp. sex"
      3 "Two adults, same sex"
      4 "Three+ related adult"
      5 "Unrelated adults"
  /HV219   
      1 "Male"
      2 "Female"
  /HV220   
     97 "97+"
     98 "DK"
  /HV221   
      0 "No"
      1 "Yes"
  /HV225   
      0 "No"
      1 "Yes"
  /HV226   
      1 "Electricity"
      2 "LPG/Natural gas"
      3 "Natural gas"
      4 "Biogas"
      5 "Kerosene"
      6 "Coal, lignite"
      7 "Charcoal"
      8 "Wood"
      9 "Straw / shrubs / grass"
     10 "Agricultural crop"
     11 "Animal dung"
     95 "No food cooked in HH"
     96 "Other"
  /HV227   
      0 "No"
      1 "Yes"
  /HV228   
      0 "No"
      1 "All children"
      2 "Some children"
      3 "No bednet in HH"
  /HV234   
      0 "0 PPM (No Iodine)"
      7 "Below 15 PPM"
     15 "15 PPM and above"
     30 "30 PPM"
    994 "Salt not tested"
    995 "No salt in household"
  /HV235   
      1 "In own dwelling"
      2 "In own yard/plot"
      3 "Elsewhere"
  /HV236   
      1 "Adult woman"
      2 "Adult man"
      3 "Female child under 15 years old"
      4 "Male child under 15 years old"
      6 "Other"
  /HV237   
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237A  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237B  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237C  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237D  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237E  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237F  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237G  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237H  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237I  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237J  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237K  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237X  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV237Z  
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HV238   
     95 "10 or more households"
     98 "Don't know"
  /HV239   
      1 "Open fire"
      2 "Open stove"
      3 "Closed stove with chimney"
      6 "Other"
  /HV240   
      0 "Neither chimney or hood"
      1 "Chimney"
      2 "Hood"
  /HV241   
      1 "In the house"
      2 "In a separate building"
      3 "Outdoors"
      6 "Other"
  /HV242   
      0 "No"
      1 "Yes"
  /HV243A  
      0 "No"
      1 "Yes"
  /HV243B  
      0 "No"
      1 "Yes"
  /HV243C  
      0 "No"
      1 "Yes"
  /HV243D  
      0 "No"
      1 "Yes"
  /HV244   
      0 "No"
      1 "Yes"
  /HV245   
     95 "95 or more"
     98 "Unknown"
  /HV246   
      0 "No"
      1 "Yes"
  /HV246A  
      0 "None"
     95 "More than 95"
     98 "Unknown"
  /HV246B  
      0 "None"
     95 "More than 95"
     98 "Unknown"
  /HV246C  
      0 "None"
     95 "More than 95"
     98 "Unknown"
  /HV246D  
      0 "None"
     95 "More than 95"
     98 "Unknown"
  /HV246E  
      0 "None"
     95 "More than 95"
     98 "Unknown"
  /HV246F  
      0 "None"
     95 "More than 95"
     98 "Unknown"
  /HV246G  
      0 "None"
     95 "More than 95"
     98 "Unknown"
  /HV246H  
      0 "None"
     95 "More than 95"
     98 "Unknown"
  /HV246I  
      0 "None"
     95 "More than 95"
     98 "Unknown"
  /HV246J  
      0 "None"
     95 "More than 95"
     98 "Unknown"
  /HV246K  
      0 "None"
     95 "More than 95"
     98 "Unknown"
  /HV247   
      0 "No"
      1 "Yes"
  /HV249   
      0 "No"
      1 "Yes"
      8 "DK"
      9 "Missing"
  /HV250   
      8 "DK"
  /HV270   
      1 "Poorest"
      2 "Poorer"
      3 "Middle"
      4 "Richer"
      5 "Richest"
  /HML1    
      7 "7+"
     98 "Don't know"
  /SHDIST  
    101 "Chitipa"
    102 "Karonga"
    103 "Nkhatabay"
    104 "Rumphi"
    105 "Mzimba"
    106 "Nkhatabay"
    201 "Kasungu"
    202 "Nkhota kota"
    203 "Ntchisi"
    204 "Dowa"
    205 "Salima"
    206 "Lilongwe"
    207 "Mchinji"
    208 "Dedza"
    209 "Ntcheu"
    210 "Lilongwe"
    301 "Mangochi"
    302 "Machinga"
    303 "Zomba"
    304 "Chiradzulu"
    305 "Blantyre"
    306 "Mwanza"
    307 "Thyolo"
    308 "Mulanje"
    309 "Phalombe"
    310 "Chikwawa"
    311 "Nsanje"
    312 "Balaka"
    313 "Neno"
    314 "Zomba"
    315 "Blantyre"
  /SHLQUEST
      1 "Chichewa"
      2 "Tumbuka"
      3 "Yao"
      4 "English"
      6 "Other"
  /SHLRESP
      1 "Chichewa"
      2 "Tumbuka"
      3 "Yao"
      4 "English"
      6 "Other"
  /SHLINT  
      1 "Chichewa"
      2 "Tumbuka"
      3 "Yao"
      4 "English"
      6 "Other"
  /SHLTRANS
      0 "Not at all"
      1 "Sometimes"
      2 "All the time"
  /SHLRESO
      5 "Mang'anja"
      6 "Lomwe"
      7 "Ndali"
      8 "Ngoni"
      9 "Nkhonde"
     10 "Lambya"
     11 "Tonga"
     12 "Sena"
     13 "Nyanja"
     14 "Sukwa"
  /SH111A2
      0 "No"
      1 "Yes"
  /SH111B  
      0 "No"
      1 "Yes"
  /SH111G  
      0 "No"
      1 "Yes"
  /SH111H  
      0 "No"
      1 "Yes"
  /SH111I  
      0 "No"
      1 "Yes"
  /SH123   
  999.5 "99.5 or more"
  999.8 "DK"
  /SH126A  
      0 "No"
      1 "Yes"
      8 "DK"
  /SH126C  
      1 "Army/police"
      2 "Other gov't worker /programme"
      3 "Private company"
      6 "Other"
      8 "DK"
  /SH138   
      1 "Blue"
      2 "Green"
      3 "White"
      6 "Other"
      8 "DK/ No preference"
  /SH139   
      1 "Conical"
      2 "Rectangular"
      8 "DK/No preference"
  /SH139A  
      1 "Observed"
      2 "No specific place"
      3 "No permission to see"
      4 "Not observed, other reason"
  /SH139B  
      0 "Water not available"
      1 "Water available"
  /SH139CA
      0 "No"
      1 "Soap or detergent (bar, liquid, powder or paste)"
  /SH139CB
      0 "No"
      1 "Ash mud sand"
  /SH139CY
      0 "No"
      1 "None"
  /SH140   
      1 "0 PPM (No Iodine)"
      2 "Below 15 PPM"
      3 "15 PPM and above"
      4 "No salt in HH"
      5 "Other: Salt not tested: no complete kit"
      6 "Salt not tested"
  /HV101   
      1 "Head"
      2 "Wife or husband"
      3 "Son/daughter"
      4 "Son/daughter-in-law"
      5 "Grandchild"
      6 "Parent"
      7 "Parent-in-law"
      8 "Brother/sister"
      9 "Co-spouse"
     10 "Other relative"
     11 "Adopted/foster child"
     12 "Not related"
     13 "Niece/nephew by blood"
     14 "Niece/nephew by marriage"
     98 "DK"
  /HV102   
      0 "No"
      1 "Yes"
  /HV103   
      0 "No"
      1 "Yes"
  /HV104   
      1 "Male"
      2 "Female"
  /HV105   
     96 "96+"
     98 "DK"
  /HV106   
      0 "No education, preschool"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
      8 "DK"
  /HV107   
     98 "DK"
  /HV108   
     97 "Inconsistent"
     98 "DK"
  /HV109   
      0 "No education"
      1 "Incomplete primary"
      2 "Complete primary"
      3 "Incomplete secondary"
      4 "Complete secondary"
      5 "Higher"
      8 "DK"
  /HV110   
      0 "No"
      1 "Yes"
  /HV111   
      0 "No"
      1 "Yes"
      8 "DK"
  /HV112   
      0 "Mother not in HH"
  /HV113   
      0 "No"
      1 "Yes"
      8 "DK"
  /HV114   
      0 "Father not in HH"
  /HV115   
      0 "Never married"
      1 "Married"
      2 "Living together"
      3 "Widowed"
      4 "Divorced"
      5 "Not living together"
  /HV116   
      0 "Never married"
      1 "Currently married"
      2 "Formerly/ever marr."
  /HV117   
      0 "Not eligible"
      1 "Eligible"
  /HV118   
      0 "Not eligible"
      1 "Eligible"
  /HV120   
      0 "Not eligible"
      1 "Eligible"
  /HV121   
      0 "No"
      1 "Currently attending"
      2 "Attended at some time"
  /HV122   
      0 "No education, preschool"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
      8 "DK"
  /HV123   
     98 "DK"
  /HV124   
     97 "Inconsistent"
     98 "DK"
  /HV125   
      0 "No"
      1 "Yes"
  /HV126   
      0 "No education, preschool"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
      8 "DK"
  /HV127   
     98 "DK"
  /HV128   
     97 "Inconsistent"
     98 "DK"
  /HV129   
      0 "Never attended"
      1 "Entered school"
      2 "Advanced"
      3 "Repeating"
      4 "Dropout"
      5 "Left school 2+ years ago"
      8 "DK"
  /HV130   
      0 "No"
      1 "Yes"
      8 "DK"
  /HV131   
      0 "No"
      1 "Yes"
      8 "DK"
  /HV132   
      0 "No"
      1 "Yes"
      8 "DK"
  /HV133   
      0 "No"
      1 "Yes"
  /HV134   
      0 "No"
      1 "Yes"
  /HV135   
      0 "No"
      1 "Yes"
      8 "DK"
  /HV136   
      0 "No"
      1 "Yes"
  /HV137   
      0 "No"
      1 "Yes"
      8 "DK"
  /HV138   
      0 "No"
      1 "Yes"
      8 "DK"
  /HV139   
      0 "No"
      1 "Yes"
      8 "DK"
  /HV140   
      0 "Neither certificate or registered"
      1 "Has certificate"
      2 "Registered"
      8 "DK"
  /SH08    
      1 "Currently married/Living together"
      2 "Divorced/Separated"
      3 "Widowed"
      4 "Never married and never lived together"
  /SH24A   
      0 "Preschool"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
      8 "DK"
  /SH26A   
      0 "Preschool"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
      8 "DK"
  /SH28A   
      0 "Preschool"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
      8 "DK"
  /SH32    
      0 "None"
      1 "1 Meal"
      2 "2 Meals"
      3 "3+ Meals"
      8 "Don't know"
      9 "Missing"
  /HA4     
   9998 "Flagged cases"
  /HA5     
   9998 "Flagged cases"
  /HA6     
  99998 "Flagged cases"
  /HA11    
   9998 "Flagged cases"
  /HA12    
  99998 "Flagged cases"
  /HA12A   
  99998 "Flagged cases"
  /HA12B   
  99998 "Flagged cases"
  /HA13    
      0 "Measured"
      3 "Not present"
      4 "Refused"
      6 "Other"
  /HA33    
      1 "Month and year"
      2 "Month and age -y imp"
      3 "Year and age - m imp"
      4 "Y & age - y ignored"
      5 "Year - a, m imp"
      6 "Age - y, m imp"
      7 "Month - a, y imp"
      8 "None - all imp"
  /HA35    
      0 "Doesn't smoke"
     80 "80+"
     94 "Smokes pipes, cigars, etc"
  /HA40    
   9998 "Flagged cases"
  /HA41    
   9998 "Flagged cases"
  /HA50    
      1 "Under age 18"
      2 "Age 18 or older"
  /HA51    
      0 "Not in household"
  /HA52    
      1 "Granted"
      2 "Parent/Other responsible refused"
      3 "Respondent refused"
  /HA54    
      0 "No/don't know"
      1 "Yes"
  /HA55    
      0 "Measured"
      3 "Not present"
      4 "Refused"
      5 ""
      6 "Other"
  /HA57    
      1 "Severe"
      2 "Moderate"
      3 "Mild"
      4 "Not anemic"
  /HA58    
      0 "No"
      1 "Yes"
  /HA60    
      1 "Never in union"
      2 "Other"
  /HA61    
      1 "Granted"
      2 "Parent/Other responsible refused"
      3 "Respondent refused"
      4 "Sample not tested/lost/not enough DBS"
  /HA63    
      1 "Blood taken"
      2 "Not present"
      3 "Refused"
      4 "Sample not tested/lost"
      5 "Not enough DBS to complete protocol"
      6 "Other"
  /HA64    
      1 "Granted"
      2 "Parent/Other responsible refused"
      3 "Respondent refused"
  /HA65    
      1 "Completed"
      2 "Not at home"
      3 "Postponed"
      4 "Refused"
      5 "Partly completed"
      6 "Incapacitated"
      7 "Other"
  /HA66    
      0 "No education"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
      8 "Don't know"
  /HA68    
      0 "No education"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
      8 "Don't know"
  /SH517   
 999.94 "Not present"
 999.95 "Refused"
 999.96 "Other"
  /SH518   
  999.4 "Not present"
  999.5 "Refused"
  999.6 "Other"
  /SH523B  
      1 "Granted"
      2 "Parent/Other responsible refused"
  /SH523D  
      1 "Granted"
      2 "Respondent refused"
  /SH525B  
      1 "Granted"
      2 "Parent/Other responsible refused"
  /SH525C  
      1 "Positive"
      2 "Negative"
      3 "Undetermined"
      4 "Refused to answer"
      6 "Blank"
  /SH525F  
      1 "Granted"
      2 "Respondent refused"
  /SH525G  
      1 "520 = 1 & 521 = 1"
      2 "Other"
  /SH525J  
      1 "Granted"
      2 "Parent/Other responsible refused"
  /SH525L  
      1 "Granted"
      2 "Respondent refused"
  /SH527   
   99.4 "Not present"
   99.5 "Refused"
   99.6 "Other"
  /HC4     
   9998 "Flagged cases"
  /HC5     
   9998 "Flagged cases"
  /HC6     
  99998 "Flagged cases"
  /HC7     
   9998 "Flagged cases"
  /HC8     
   9998 "Flagged cases"
  /HC9     
  99998 "Flagged cases"
  /HC10    
   9998 "Flagged cases"
  /HC11    
   9998 "Flagged cases"
  /HC12    
  99998 "Flagged cases"
  /HC13    
      0 "Measured"
      3 "Not present"
      4 "Refused"
      6 "Other"
  /HC15    
      1 "Lying"
      2 "Standing"
  /HC16    
     97 "Inconsistent"
     98 "DK"
  /HC27    
      1 "Male"
      2 "Female"
  /HC30    
     97 "Inconsistent"
     98 "DK"
  /HC31    
   9997 "Inconsistent"
   9998 "DK"
  /HC33    
      1 "Month and year"
      2 "Month and age"
      3 "Year and age"
      4 "Year"
      5 ""
      6 "Age"
      7 "Month"
      8 "None"
  /HC51    
      0 "Not in household"
  /HC52    
      1 "Granted"
      2 "Refused"
  /HC55    
      0 "Measured"
      3 "Not present"
      4 "Refused"
      5 ""
      6 "Other"
  /HC57    
      1 "Severe"
      2 "Moderate"
      3 "Mild"
      4 "Not anemic"
  /HC58    
      0 "No"
      1 "Yes"
  /HC60    
    993 "Mother not de facto"
    994 "Incomplete woman's interview"
    995 "Not in household"
  /HC61    
      0 "No education"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
  /HC68    
      0 "No education"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
  /HC70    
   9996 "Height out of plausible limits"
   9997 "Age in days out of plausible limits"
   9998 "Flagged cases"
  /HC71    
   9996 "Height out of plausible limits"
   9997 "Age in days out of plausible limits"
   9998 "Flagged cases"
  /HC72    
   9996 "Height out of plausible limits"
   9997 "Age in days out of plausible limits"
   9998 "Flagged cases"
  /HC73    
   9996 "Height out of plausible limits"
   9997 "Age in days out of plausible limits"
   9998 "Flagged cases"
  /SH505   
  99.94 "Not present"
  99.95 "Refused"
  99.96 "Other"
  /SH506   
  999.4 "Not present"
  999.5 "Refused"
  999.6 "Other"
  /SH507   
      1 "Lying"
      2 "Standing"
      3 "Not measured"
  /SH512   
   99.4 "Not present"
   99.5 "Refused"
   99.6 "Other"
  /HB4     
   9998 "Flagged cases"
  /HB5     
   9998 "Flagged cases"
  /HB6     
  99998 "Flagged cases"
  /HB11    
   9998 "Flagged cases"
  /HB12    
  99998 "Flagged cases"
  /HB12A   
  99998 "Flagged cases"
  /HB12B   
  99998 "Flagged cases"
  /HB13    
      0 "Measured"
      3 "Not present"
      4 "Refused"
      5 ""
      6 "Other"
  /HB33    
      1 "Month and year"
      2 "Month and age -y imp"
      3 "Year and age - m imp"
      4 "Y & age - y ignored"
      5 "Year - a, m imp"
      6 "Age - y, m imp"
      7 "Month - a, y imp"
      8 "None - all imp"
  /HB35    
      0 "Doesn't smoke"
     80 "80+"
     94 "Smokes pipes, cigars, etc"
     98 "Don't know"
  /HB40    
   9998 "Flagged cases"
  /HB41    
   9998 "Flagged cases"
  /HB50    
      1 "Under age 18"
      2 "Age 18 or older"
  /HB51    
      0 "Not in household"
  /HB52    
      1 "Granted"
      2 "Parent/Other responsible refused"
      3 "Respondent refused"
  /HB55    
      0 "Measured"
      3 "Not present"
      4 "Refused"
      5 ""
      6 "Other"
  /HB57    
      1 "Severe"
      2 "Moderate"
      3 "Mild"
      4 "Not anemic"
  /HB58    
      0 "No"
      1 "Yes"
  /HB60    
      1 "Never in union"
      2 "Other"
  /HB61    
      1 "Granted"
      2 "Parent/Other responsible refused"
      3 "Respondent refused"
      4 "Sample not tested/lost/not enough DBS"
  /HB63    
      1 "Blood taken"
      2 "Not present"
      3 "Refused"
      4 "Sample not tested/lost"
      5 "Not enough DBS to complete protocol"
      6 "Other"
  /HB64    
      1 "Granted"
      2 "Parent/Other responsible refused"
      3 "Respondent refused"
  /HB65    
      1 "Completed"
      2 "Not at home"
      3 "Postponed"
      4 "Refused"
      5 "Partly completed"
      6 "Incapacitated"
      7 "Other"
  /HB66    
      0 "No education"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
      8 "Don't know"
  /HB68    
      0 "No education"
      1 "Primary"
      2 "Secondary"
      3 "Higher"
      8 "Don't know"
  /SH533   
      1 "Present"
      2 "Not present"
  /SH540B  
      1 "Granted"
      2 "Parent/Other responsible refused"
  /SH540C  
      1 "Positive"
      2 "Negative"
      3 "Undetermined"
      4 "Refused to answer"
      6 "Blank"
  /SH540F  
      1 "Granted"
      2 "Respondent refused"
  /SH540G  
      1 "15-17 years"
      2 "18-49"
  /SH540J  
      1 "Granted"
      2 "Parent/Other responsible refused"
  /SH540L  
      1 "Granted"
      2 "Respondent refused"
  /HML3    
      0 "Not seen"
      1 "Yes, seen"
  /HML4    
     96 "More than 3 years ago"
     98 "Don't know"
  /HML5    
      0 "No"
      1 "Yes"
      8 "Don't know"
  /HML6    
      0 "Not pretreated"
      1 "Pretreated, permanent tx"
      2 "Pretreated, requiring future tx"
      3 "Not pretreated, came with kit and treated at home"
      4 "Pretreated, treatment type not known"
      6 "Other"
      8 "Don't know"
  /HML7    
     11 "ITN/ long-lasting: duranet"
     12 "ITN/ long-lasting: olysnet"
     13 "ITN/ long-lasting: lifenet"
     14 "ITN/ long-lasting: permanet"
     16 "ITN/ long-lasting: other/ DK brand"
     21 "Retreatable: safi net"
     26 "Retreatable: other/ DK brand"
     31 "Untreated: safi net"
     36 "Untreated: other/ DK brand"
     96 "Other"
     98 "DK Brand"
  /HML8    
      0 "No"
      1 "Yes"
      2 "Permanent net"
      8 "Not sure"
  /HML9    
     95 "25+ months ago"
     96 "More than 3 years ago"
     98 "Don't know"
  /HML10   
      0 "No, don't know"
      1 "Yes"
  /HML11   
      5 "5+"
  /HML21   
      0 "No"
      1 "Yes"
      8 "DK"
  /HMLA    
      0 "No one"
  /SH129A  
      0 "No"
      1 "Yes"
  /SH129B  
      1 "Green"
      2 "Dark blue"
      3 "Light blue"
      4 "White"
      6 "Other"
  /SH129C  
      1 "Conical"
      2 "Rectangle"
  /SH130C  
      0 "No"
      1 "Yes"
      8 "Not sure"
  /HML12   
      0 "No bednet"
      1 "Only treated bednets (ITN)"
      2 "Both treated (ITN) and untreated bednets"
      3 "Only untreated bednets"
  /HML13   
      0 "Did not sleep under net"
  /HML16   
     97 "97+"
     98 "DK"
  /HML17   
      0 "No data from individual questionnaire"
      1 "Month and year"
      2 "Month and age -y imp"
      3 "Year and age - m imp"
      4 "Y & age - y ignored"
      5 "Year - a, m imp"
      6 "Age - y, m imp"
      7 "Month - a, y imp"
      8 "None - all imp"
  /HML18   
      0 "Not pregnant, don't know"
      1 "Pregnant"
  /HML19   
      0 "No"
      1 "Yes"
  /HS100   
      0 "No"
      1 "Yes"
      8 "DK"
  /HS101   
      0 "No"
      1 "Yes"
      8 "DK"
  /HS102   
      0 "No"
      1 "Yes"
      8 "DK"
  /HS103   
      0 "No"
      1 "Yes"
      8 "DK"
  /HS104   
      0 "No"
      1 "Yes"
      8 "DK"
  /HS105   
      0 "No"
      1 "Yes"
      8 "DK"
  /HS106   
      0 "No"
      1 "Yes"
      8 "DK"
  /HS107   
      0 "No"
      1 "Yes"
      8 "DK"
  /HS108   
      0 "Not at all"
      1 "Severe"
      2 "Mild"
      8 "DK"
  /HS109   
      0 "Not at all"
      1 "Most of the time"
      2 "Some time"
  /HS110   
      0 "No"
      1 "Yes, severe"
      2 "Yes, never severe"
  /HS111   
      0 "Not at all"
      1 "Most of the time"
      2 "Some time"
  /HO101   
      0 "No"
      1 "Yes"
      8 "DK"
  /HO102   
      0 "No"
      1 "Yes"
      8 "DK"
  /HO103   
      0 "No"
      1 "Yes"
      8 "DK"
  /HO104   
      0 "No"
      1 "Yes"
      8 "DK"
  /HO105   
      0 "No"
      1 "Yes"
      8 "DK"
  /HO106   
      0 "No"
      1 "Yes"
      8 "DK"
  /HO107   
      0 "No"
      1 "Yes"
      8 "DK"
  /HO108   
      0 "No"
      1 "Yes"
      8 "DK"
  /SH416AA
      0 "No"
      1 "Money for school fees"
  /SH416AB
      0 "No"
      1 "Other money"
  /SH416AC
      0 "No"
      1 "Uniform"
  /SH416AD
      0 "No"
      1 "Notebooks"
  /SH416AX
      0 "No"
      1 "Other"
