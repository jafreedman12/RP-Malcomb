---
layout: page
title: RP- Vulnerability modeling for sub-Saharan Africa
---


**Replication of**
# Vulnerability modeling for sub-Saharan Africa

Original study *by* Malcomb, D. W., E. A. Weaver, and A. R. Krakowka. 2014. Vulnerability modeling for sub-Saharan Africa: An operationalized approach in Malawi. *Applied Geography* 48:17–30. DOI:[10.1016/j.apgeog.2014.01.004](https://doi.org/10.1016/j.apgeog.2014.01.004)

Replication Authors:
Jacob Freedman, Joseph Holler, Kufre Udoh, Open Source GIScience students of fall 2019 and Spring 2021

Replication Materials Available at: [RP-Malcomb](https://github.com/jafreedman12/RP-Malcomb)

Created: `12 April 2021`
Revised: `27 April 2021`

## Abstract

The original study is a multi-criteria analysis of vulnerability to Climate Change in Malawi, and is one of the earliest sub-national geographic models of climate change vulnerability for an African country. The study aims to be replicable, and had 40 citations in Google Scholar as of April 8, 2021.

## Original Study Information

The study region is the country of Malawi. The spatial support of input data includes DHS survey points, Traditional Authority boundaries, and raster grids of flood risk (0.833 degree resolution) and drought exposure (0.416 degree resolution).

The original study was published without data or code, but has detailed narrative description of the methodology. The methods used are feasible for undergraduate students to implement following completion of one introductory GIS course. The study states that its data is available for replication in 23 African countries.


## Data Description and Variables
This component was written collaboratively with Alitzel Villanueva, Maja Cannavo, Emma Clinton, Drew An-Pham, and Nick Nonnenmacher, all students in GEOG0323.

Outline the data used in the study, including:

- sources of each data layer and
- the variable(s) used from each data source
- transformations applied to the variables (e.g. rescaling variables, calculating derived variables, aggregating to different geographic units, etc.)

### Assets and Access:
Demographic and Health Survey data are a product of the United States Agency for International Development (USAID). Variables contained in this dataset are used to represent adaptive capacity (access + assets) in the Malcomb et al.’s (2014) study. These data come from survey questionnaires with large sample sizes.

The DHS data used in our study were collected in 2010. In Malawi, the provenance of the DHA data dates back as far as 1992, but has not been collected consistently every year. Each point in the household dataset represents a cluster of households with each cluster corresponding to some form of census enumeration units, such as villages in rural areas or city blocks in urban areas [DHS GPS Manual](/data/metadata/DHS_GPS_Manual_English_A4_24May2013_DHSM9.pdf). This means that each household in each cluster has the same GPS data. This data is collected by trained [USAID](https://www.usaid.gov/) staff using GPS receivers.

Missing data is a common occurrence in this dataset as a result of negligence or incorrect naming. However, according to the [DHS GPS Manual](/data/metadata/DHS_GPS_Manual_English_A4_24May2013_DHSM9.pdf), these issues are easily rectified and typically sites for which data does not exist are recollected. Sometimes, however, missing information is coded in as such or assigned a proxy location.

The DHS website acknowledges the high potential for inconsistent or incomplete data in such broad and expansive survey sets. Missing survey data (responses) are never estimated or made up; they are instead coded as a special response indicating the absence of data. As well, there are clear policies in place to ensure the data’s accuracy. More information about data validity can be found on the [DHS’s Data Quality and Use site](https://www.dhsprogram.com/data/Data-Quality-and-Use.cfm).

In this analysis, we use the variables listed in **Table 1** to determine the average adaptive capacity of each TA area. Data transformations are outlined below.

***Table 1: Variables from DHS data***
| Variable Code  | Definition  |
| ------------- | ------------- |
| HHID  | "Case Identification"  |
| HV001  | "Cluster number"  |
|HV002  | Household number  |
| HV246A  |"Cattle own"  |
|HV246D  | "Goats own"  |
|HV246E  | "Sheep own"  |
|HV246G  | "Pigs own"  |
| HV248  |"Number of sick people 18-59"  |
| HV245  | "Hectares for agricultural land"  |
|HV271  | "Wealth index factor score (5 decimals)"  |
|HV251  | "Number of orphans and vulnerable children"  |
|HV207  | “Has Radio”  |
| HV243A  | “Has a Mobile Telephone”  |
|HV219  | Sex of Head of Household”  |
|HV226  | “Type of Cooking Fuel”  |
| HV206  |"Has electricty”  |
|HV204  |“Time to get to Water Source”  |



### Livelihood Zones:

The Livelihood zone data is created by aggregating general regions where similar crops are grown and similar ecological patterns exist. This data exists originally at the household level and was aggregated into Livelihood Zones. To construct the aggregation used for “Livelihood Sensitivity” in this analysis, we use these household points from the FEWSnet data that had previously been aggregated into livelihood zones. The four Livelihood Sensitivity categories are 1) Percent of food from own farm (6%); 2) Percent of income from wage labor (6%); 3) Percent of income from cash crops (4%); and 4) Disaster coping strategy (4%). In the original R script, household data from the DHS survey was used as a proxy for the specific data points in the livelihood sensitivity analysis (transformation: Join with DHS clusters to apply LHZ FNID variables). With this additional FEWSnet data at the household level, we can construct these four livelihood sensitivity categories using existing variables (Table 1).

The LHZ data variables are outlined in **Table 2**. The four categories used to determine livelihood sensitivity were ranked from 1-5 based on percent rank values and then weighted using values taken from Malcomb et al. (2014).

***Table 2: Constructing livelihood sensitivity categories***
| Livelihood Sensitivity Category (LSC)  | Percent Contributing  | How LSC was constructed  |
| ------------- | ------------- | ------------- |
| Percent of food from own farm  |  6%  | Sources of food: crops + livestock  |
| Percent of income from wage labor  | 6%  | Sources of cash: labour etc. / total * 100  |
| Percent of income from cash crops  | 4%  | sources of cash (Crops): (tobacco + sugar + tea + coffee) + / total sources of cash * 100  |
| Disaster coping strategy  | 4%  | Self-employment & small business and trade: (firewood + sale of wild food + grass + mats + charcoal) / total sources of cash * 100  |


### Physical Exposure: Physical exposition to droughts events 1980-2001
This dataset uses the Standardized Precipitation Index to measure annual drought exposure across the globe. The Standardized Precipitation Index draws on data from a “global monthly gridded precipitation dataset” from the University of East Anglia’s Climatic Research Unit, and was modeled in GIS using methodology from Brad Lyon at Columbia University. The dataset draws on 2010 population information from the LandScanTM Global Population Database at the Oak Ridge National Laboratory.  Drought exposure is reported as the expected average annual (2010) population exposed. The data were compiled by UNEP/GRID-Europe for the Global Assessment Report on Risk Reduction (GAR). The data use the WGS 1984 datum, span the years 1980-2001, and are reported in raster format with spatial resolution 1/24 degree x 1/24 degree.



### Analytical Specification

The original study was conducted using ArcGIS and STATA, but does not state which versions of these software were used.
The replication study will use R.

## Materials and Procedure

### ADAPTIVE CAPACITY WORKFLOW [ASSETS & ACCESS]
1. Bring in DHS Data [Households Level] (vector)
2. Bring in TA (Traditional Authority boundaries) and LHZ (livelihood zones) data
3. Get rid of unsuitable households (eliminate NULL and/or missing values)
3. Join TA and LHZ ID data to the DHS clusters
4. Pre-process the livestock data
	Filter for NA livestock data
	Update livestock data (summing different kinds)
5. FIELD CALCULATOR: Normalize each indicator variable and rescale from 1-5 (real numbers) based on percent rank
6. FIELD CALCULATOR / ADD FIELD: Apply weights to normalized indicator variables to get scores for each category (assets, access)
7. SUMMARIZE/AGGREGATE: find the stats of the capacity of each TA (min, max, mean, sd)
8. Join ta_capacity to TA based on ta_id
	(Multiply by 20--meaningless??) I have a question about this (so do I) ln.216
9. Prepare breaks for mapping
Class intervals based on capacity_2010 field
Take the values and round them to 2 decimal places
Put data in 4 classes based on break values
10. Save the adaptive capacity scores

11. Load in UNEP raster
Set CRS for drought
Set CRS for flood
12.  Clean and reproject rasters
Create a bounding box at extent of Malawi Where does this info come from
Add geometry info and precision (st_as_sfc)
For Drought: use bilinear to avg continuous population exposure values
For Flood: use nearest neighbor to preserve integer values
13. CLIP the traditional authorities with the LHZs to cut out the lake
14. RASTERIZE the ta_capacity data with pixel data corresponding to capacity_2010 field
15. RASTER CALCULATOR:
Create a mask
Reclassify the flood layer (quintiles, currently binary)
Reclassify the drought values (quantile [from 0 - 1 in intervals of 0.2 =5])
Add component rasters for final weighted score of drought + flood
16. AGGREGATE: Create final vulnerability layer using envi. vulnerability score and ta_capacity I’m a little confused about how exactly this happens, but seems to be averaging the ta_final (which corresponds to vulnerability) and ta_2010 columns

Also, where does LHZ enter into this final value?


## Replication Results
The code used for this replication can be found [here](https://github.com/jafreedman12/RP-Malcomb/blob/main/procedure/code/RP-Malcomb-jf.Rmd).


For each output from the original study (mainly figure 4 and figure 5), present separately the results of the replication attempt.

2.	State whether the original study was or was not supported by the replication
3.	State whether any hypothesis linked to a planned deviation from the original study was supported. Provide key statistics and related reasoning.

Figures to Include:

### Figure 4: Adaptive Capacity
***map of resilience by traditional authority in 2010, analagous to figure 4 of the original study***
![Replication of Fig. 4: Adaptive capacity scores](https://github.com/jafreedman12/RP-Malcomb/blob/main/results/maps/ac_2010.png)

***map of difference between your figure 4 and the original figure 4***
![Difference between Fig. 4 by Malcomb et al. (2014) and by replication](https://github.com/jafreedman12/RP-Malcomb/blob/main/results/maps/difference_ac_2010.png)

***Confusion Matrix***
| 1  | 2  | 3  | 4  |
| ------------- | ------------- |
| 1  | 35  | 5  | 0  | 0  |
| 2  | 27  | 26  | 0  | 0  |
| 3  | 5  | 44  | 19  | 0  |
| 4  | 0  | 7  | 28  | 4  |

***Spearman's Rho coefficients:***
Spearman's Rho, Comparing figure 4: 0.7861



### Figure 5: Vulnerability to Climate Change
***map of vulnerability in Malawi, analogous to figure 5 of the original study***
![Replication of Fig. 5: Vulnerability to climate disasters](https://github.com/jafreedman12/RP-Malcomb/blob/main/results/maps/vulnerability.png)

***map of difference between your figure 5 and the original figure 5***
![Difference between Fig. 5 by Malcomb et al. (2014) and by replication](https://github.com/jafreedman12/RP-Malcomb/blob/main/results/maps/difference_vulnerability.png)


***Scatterplot of difference of results for Fig. 5***
![Scatterplot of difference of results from Figure 5](https://github.com/jafreedman12/RP-Malcomb/blob/main/results/figures/fig5_diff_scatterplot.png)

***Spearman's Rho coefficients:***
Spearman's Rho, Comparing figure 5: 0.0603



## Unplanned Deviations from the Protocol

Summarize changes and uncertainties between
- your interpretation and plan for the workflow based on reading the paper
- your final workflow after accessing the data and code and completing the code

## Discussion

Provide a summary and interpretation of the key findings of the replication *vis-a-vis* the original study results. If the attempt was a failure, discuss possible causes of the failure. In this replication, any failure is probably due to practical causes, which may include:
- lack of data
- lack of code
- lack of details in the original analysis
- uncertainties due to manner in which data has been used

## Conclusion

Restate the key findings and discuss their broader societal implications or contributions to theory.
Do the research findings suggest a need for any future research?

## References

Malcomb, D. W., E. A. Weaver, and A. R. Krakowka. 2014. Vulnerability modeling for sub-Saharan Africa: An operationalized approach in Malawi. Applied Geography 48:17–30. DOI:10.1016/j.apgeog.2014.01.004

Tate, E. 2013. Uncertainty Analysis for a Social Vulnerability Index. Annals of the Association of American Geographers 103 (3):526–543. doi:10.1080/00045608.2012.700616.


####  Report Template References & License

This template was developed by Peter Kedron and Joseph Holler with funding support from HEGS-2049837. This template is an adaptation of the ReScience Article Template Developed by N.P Rougier, released under a GPL version 3 license and available here: https://github.com/ReScience/template. Copyright © Nicolas Rougier and coauthors. It also draws inspiration from the pre-registration protocol of the Open Science Framework and the replication studies of Camerer et al. (2016, 2018). See https://osf.io/pfdyw/ and https://osf.io/bzm54/

Camerer, C. F., A. Dreber, E. Forsell, T.-H. Ho, J. Huber, M. Johannesson, M. Kirchler, J. Almenberg, A. Altmejd, T. Chan, E. Heikensten, F. Holzmeister, T. Imai, S. Isaksson, G. Nave, T. Pfeiffer, M. Razen, and H. Wu. 2016. Evaluating replicability of laboratory experiments in economics. Science 351 (6280):1433–1436. https://www.sciencemag.org/lookup/doi/10.1126/science.aaf0918.

Camerer, C. F., A. Dreber, F. Holzmeister, T.-H. Ho, J. Huber, M. Johannesson, M. Kirchler, G. Nave, B. A. Nosek, T. Pfeiffer, A. Altmejd, N. Buttrick, T. Chan, Y. Chen, E. Forsell, A. Gampa, E. Heikensten, L. Hummer, T. Imai, S. Isaksson, D. Manfredi, J. Rose, E.-J. Wagenmakers, and H. Wu. 2018. Evaluating the replicability of social science experiments in Nature and Science between 2010 and 2015. Nature Human Behaviour 2 (9):637–644. http://www.nature.com/articles/s41562-018-0399-z.
