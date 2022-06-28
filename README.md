# PISA2012 Data Analysis
## by Dingdong Li


## PISA 2012
 The dataset that I analysed is the OECD’s Programme for International Student Assessment 2012 survey dataset (PISA2012). The survey assessed the 15-year-old students' skills and knowledge in mathematics, science and reading. Around 510,000 students in 65 economies took part in the PISA 2012 assessment of reading, mathematics and science. Of those economies, 44 took part in an assessment of creative problem solving and 18 in an assessment of financial literacy. 

### Structure of the dataset:

The original PISA2012 dataset has 485,490 rows and 636 columns. The datatypes of columns are float (250 columns), integer (18 columns) and object (368 columns). The metadata are provided by the pisa2012disc.txt. The columns includes the students basic information, like the country, which school they attend, gender, age and so forth, their answers to the questionairs, the integrated results of different measures infered from the answers of the questionairs (for example, Disciplinary climate (DISCLIMA) is based on all five items in ST81), five plausible values of the student performance in the mathematica, science and reading, weights and dataentry date.
### The main feature(s) of interest:

I am mainly interested in how the immigration status and family environment contribute to the students' math, reading and science performance in the United States. 

### Feature of interests:

- CNT:	Country code 3-character
- SCHOOLID:	School ID 7-digit (region ID + stratum ID + 3-digit school ID)
- STIDSTD:	Student ID
- ST04Q01:	Gender
- IMMIG: immigrant background
- FAMSTRUC:	Family Structure
- BFMJ2: father’s occupational status
- BMMJ1: mother’s occupational status
- HISEI: the highest occupational status of parents 
- FISCED: educational level of father 
- MISCED: educational level of mother 
- HISCED: highest educational level of parents
- PARED:  Highest parental education in years
- OUTHOURS:	Out-of-School Study Time
- PV1MATH:	Plausible value 1 in mathematics
- PV1READ:	Plausible value 1 in reading
- PV1SCIE:	Plausible value 1 in science

## Summary of Findings

First, I did some data pre-wrangling to fix the datatypes and column names and select only the student of United States. Then, I applied univariant exploration on my dataset to look at the distribution of each feature. 

Next, I investigate the bivarient relationships between the features, I found that the student's math science and reading scores have strong positive correlation with each other and the parents occupational status and educational level are also positively correlated with the students academic performance.

Finally, I looked at how the gender, family strucure, immigration status can affect the relationship between students' academic performance and parents occupational status. It has been shown that the gender doesn't affect the so much the relationship. The family structure does affect this relationship. In the two-parents family, the regression slope is largest, then is the single-parent family. The students who don't live with their parents, their academic performance doesn't correlate with the parents occupational status.
## Key Insights for Presentation
- 
