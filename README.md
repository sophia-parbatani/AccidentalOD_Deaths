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
# Manipulations for the Heat Map

- Filtered records to include only confirmed overdose cases (drug involvement = 'Y') — to focus the analysis on relevant incidents by applying a filter condition.
- Pivoted drug columns into a single “Drug Type” field — to allow comparison across substances by consolidating multiple drug columns into one using pivot functionality.
- Created age bins in 10-year intervals — to group individuals for demographic analysis by generating calculated age ranges.
- Counted records by age, sex, and drug — to measure overdose frequency across categories by aggregating grouped data.
- Renamed fields and applied aliases — to improve clarity and presentation by updating field labels (e.g., “10” → “0–10”).

# Analysis & Results of Heap Map

Using Tableau, we created heat maps and charts to visualize patterns in fentanyl-related overdoses across counties and demographic groups.

__Insights:__
Our county-level heat map revealed overdose clusters, showing where interventions like public health campaigns, treatment centers, and naloxone distribution should be focused.
Demographic Insights (from overdose trends chart):
Males aged 21–40 have the highest number of fentanyl-related overdoses, with over 1,700 cases in the 21–30 group alone.
Females aged 30–50 are most affected by benzodiazepines and cocaine overdoses.
These trends support the need for age- and gender-targeted interventions.

__Implications ->__

__Prevention__: Educational outreach, including mental health campaigns like #MentionPrevention

__Policy & Resources__: Expand access to treatment centers, counseling, naloxone, and recovery support

__Early Intervention__: Implement overdose awareness in schools and colleges, especially for at-risk age groups

__Source: CDC WONDER – https://wonder.cdc.gov__ 

# Manipulations for the Zone Map
- Created a new “record count” field to calculate total overdose deaths by counting entries in the dataset.
- Used generated longitude and latitude to map each case geographically, filtered specifically for fentanyl-related overdoses.
- Applied color encoding to show the percentage each county contributed to total fentanyl overdoses.
- Displayed text labels to show the number of deaths and corresponding county names for clarity.

# Analysis & Results of Zone Map
We used Tableau to create a zone (choropleth) map visualizing fentanyl-related overdose deaths across counties in Connecticut. The map was filtered to include only fentanyl cases, with generated latitude and longitude used for geographic accuracy. Color intensity represents the percentage of total fentanyl deaths by county, and labels display the exact death counts.

__Insights:__

New Haven (2,126 deaths) and Hartford (2,110 deaths) are the two leading counties for fentanyl-related deaths.
Together, they account for nearly 25% of all drug-related deaths in the dataset, signaling a major urban concentration of overdose cases.
These counties have high population density and urban infrastructure, which may contribute to greater drug availability, socioeconomic stress, and limited healthcare access.

__Implications ->__

Intervention efforts—such as naloxone distribution, addiction treatment centers, and public health education—should be prioritized in urban counties like Hartford and New Haven.
Geographic visualizations like this help localize resource planning and improve response effectiveness.

__Source: CDC WONDER – https://wonder.cdc.gov__
