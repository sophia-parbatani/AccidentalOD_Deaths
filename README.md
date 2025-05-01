# Accidental_OD_Deaths
Analysis of trends amongst accidental overdoses in Connecticut
# Team name and members
(Team 6) Ari Pais, Esom Nwachukwu, Reya Harees, Sophia Parbatani, Ian Wright
# Data Set Information
11,982 rows and 48 columns
The notable categorical data: sex, race, county, manner of death: (accidental/intentional), type of drug for the OD
The quantitative data to note: age, number of deaths
![image](https://github.com/user-attachments/assets/13d01148-403b-4a23-8df4-c41cde18f6a3)
# Why did we choose this data?
Accidental drug overdoses are the most common type of drug-related death, with 65.9% involving at least one missed opportunity for intervention (CDC.gov). The ongoing fentanyl crisis has intensified the urgency of this issue. Accidental ODs affect a broad range of demographics, but the risk begins to rise rapidly in our 20s, peaking around age 36—making this data especially relevant to our generation.
# Our Questions and why they are important
1) __Is there a trend among age and sex relevant to drug that causes the OD?__
	
 - Clusters of a population often frequent the same areas/activities

- Ex.) 16 yr old male/female – this cluster commonly attends high school

- Targeted resources/intervention for the specific drug affecting given population the most


2) __What proportion of total accidental ODs show traces of fentanyl in the tox screen? Does this vary by county?__

 - The head of the U.S. Drug Enforcement Administration (DEA), Anne Milgram, said that “fentanyl is the single deadliest drug threat our nation has ever encountered.”

- Fentanyl is the top killer among all demographics in drug overdose deaths

- Finding the locations where fentanyl is most common in tox screens could indicate problem areas to public health officials as well as law enforcement. 

- Higher percentage tox containing trace amounts of fentanyl = possible import/activity hotspots
# Manipulations in the datset

- Filtered records to include only confirmed overdose cases (drug involvement = 'Y') — to focus the analysis on relevant incidents by applying a filter condition.
- Pivoted drug columns into a single “Drug Type” field — to allow comparison across substances by consolidating multiple drug columns into one using pivot functionality.
- Created age bins in 10-year intervals — to group individuals for demographic analysis by generating calculated age ranges.
- Counted records by age, sex, and drug — to measure overdose frequency across categories by aggregating grouped data.
- Renamed fields and applied aliases — to improve clarity and presentation by updating field labels (e.g., “10” → “0–10”).


