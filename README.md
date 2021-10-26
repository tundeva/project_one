[A] SCOPE
Exhaustive 3-dimensional Analysis to comparatively quantify the beneficial effects of Mask Mandates, weighted against per capital income of respective US localities.

[B] CORE OBJECTIVE
To answer the question: Did a factor like per capital income contribute to the effectiveness of Mask Mandates or it never mattered at all so long as Mask Mandates were uniformly enforced in the local population?

[C] BACKGROUND INFORMATION
The Severe Acute Respiratory Syndrome Corona Virus (SARS COV-2, also known as Covid 19 began spreading - as a matter of serious Public Health significance - in the United States in the first quarter of 2020. The consensus among Public Health experts as to its mode of propagation is that Covid 19 is infectious and it spreads from person-to-person. Therefore, to mitigate its spread, so-called Mask Mandates were instituted at different times and to different degrees by local public health authorities.
It is a known fact that Mask Mandates help with reducing the spread of covid 19. CDC data models seem to firmly support that consensus.
However, as is common knowledge as at the time of this study, certain factors affect Covid 19 propagation and outcomes, chiefly among these is the issue of patient comorbidities, which include Obesity, High Blood Pressure, Diabetes, HIV, Cancer treatments, Organ Transplantation etc. Most of these factors, and the effective management of them prior to infection directly relate to income level and general quality of life.
Covid 19 seeks to overwhelm an individual’s immune system by producing spike proteins. Presumably, majority of people who get infected never realize they were infected unless they are immune-compromised due to extraneous factors e.g., the presence of a comorbidity.
Therefore it is quite possible that Mask Mandates may actually work better in areas where people have higher quality of life and access to quality medical care, simply because many Covid 19 infections, in spite of the mandates, may have gone unreported, relative to areas with poorer conditions of life.
This analysis will employ the skill set and tools acquired in the course of Georgia Tech Data Science Course to gauge the relative benefit of the Mandates, when correlated with income.

[D] DATA SETS
1)  mandates_by_county.csv (From group mates)
2) social_vulnerability_data (From CDC)
3) covid_related_deaths_by_county – (From CDC)

[E] METHODOLOGY
Step 1
Using Panda binnings, we shall group counties into clusters, depending on the ratio of mask days to total days.
1)	County Cluster 1: less than 0 – 10% Mandate (i.e Counties that imposed Mask Mandates less that 10% of total days in period of data)
2)	County Cluster 2: 10% - 20%
3)	County Cluster 3: 20% - 30%
4)	County Cluster 4: 30% - 40%
5)	County Cluster 5: 40% - 50%
6)	County Cluster 6: 50% - 60%
7)	County Cluster 7: 60% - 70%
8)	County Cluster 8: 70% - 80%
9)	County Cluster 9: Over 80%

Step 2 
 Merge the 3 data sets using State and county Information as commonality
Step 3
Extract Loc Frames based on bins, out of merged data set.
Step 4
Plot Scatterplots based on extracted bins.

[F] CONSIDERATIONS TO NOTE
(1) The incubation period of Sars Cov-2, from infection to severity/hospitalization is thought to be around 14 days, with 4 to 5 days being the median from infection to beginning of symptoms. Source: CDC. https://www.cdc.gov/coronavirus/2019-ncov/hcp/clinical-guidance-management-patients.html
(2) Other factors like lock downs and stay-at-home orders which occurred in many cases simultaneously with Mask Mandates may have helped mitigate severity. Our analysis model must factor in these other factors.
(3) People with co-morbidity, like High Blood Pressure, Diabetes, Obesity, Cancer, HIV and a history of Organ Transplantation are more vulnerable to the debilitating effects of Sars Cov-2 than people without such underlying health challenges.
(4) Age of the patient is a factor when gauging expected vulnerability to Sars Cov-2.
(5) We will limit our analysis to within periods before vaccines became available.



[G] CONCLUSION
The scatterplots that will emerge will be representative of income to mortality data which has been modularized into bins based on degree of Mask mandates. If there is a discernable pattern that tend to show a trending relationship between per-capital income of residents of counties within that bin and rate of covid-related deaths, then we shall conclude that mask mandates are more effective or less effective with increasing or decreasing income.

