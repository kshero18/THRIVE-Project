# THRIVE-Project

**THRIVE Data Analyst Findings Report**

*Global Hunger Index Analysis*

Prepared by: Shiro

Date: January 2026

*Data Sources*
This analysis uses two open-access datasets from Our World in Data (OWID): Global Hunger Index and Global Hunger Index vs GDP per Capita. OWID aggregates and standardises data from reputable international organisations, making it suitable for cross-country comparison and exploratory analysis of global socio-economic issues.

*Data Preparation and Cleaning*
Both datasets were loaded using Python and cleaned prior to analysis. The Year column was coerced into numeric format to ensure correct filtering and time-based operations. Key indicator columns, including the Global Hunger Index (GHI) and GDP per capita, were also converted to numeric values with invalid entries handled as missing data. To maintain consistency and avoid aggregation errors, the analysis was restricted to country-level entities by filtering for valid ISO-3 country codes. This removed regions and aggregates that could otherwise bias the results.

*Visualisation Choices and Rationale*
Four visual outputs were produced to address different analytical perspectives:

1.	Top 10 Countries by Global Hunger Index (2021)
A horizontal bar chart was used to clearly rank countries with the highest hunger severity in 2021. This format allows for easy comparison and highlights the countries most affected by hunger.

2.	Global Hunger Index vs GDP per Capita (Scatter Plot)
A scatter plot was selected to explore the relationship between economic prosperity and hunger outcomes. This visual helps assess whether higher GDP per capita generally corresponds to lower hunger levels, and to identify outliers.

3.	Average Global Hunger Index by Continent (2021)
Aggregating GHI scores by continent provides a regional perspective, revealing broad geographic disparities in hunger levels. A horizontal bar chart was used for clarity and readability.

4.	Animated Racing Bar Chart (Selected Countries Over Time)
The racing chart visualises changes in GHI across multiple years for selected countries. This dynamic format effectively communicates long-term trends and relative progress or deterioration over time.

*Key Challenges*

A notable challenge was incomplete metadata coverage in the GDP dataset, particularly for recent years and continent labels. This required careful handling of missing values and the use of reference-year metadata to enable continent-level analysis. These limitations were transparently documented and did not undermine the overall insights.

*Key Insights*

The analysis shows that countries with the highest GHI scores in 2021 are predominantly low-income or conflict-affected nations. The scatter plot suggests an inverse relationship between GDP per capita and hunger severity, although notable exceptions exist. Continent-level averages highlight higher hunger burdens in Africa and parts of Asia. The animated chart demonstrates that progress over time is uneven, with some countries showing improvement while others experience stagnation or reversal.
