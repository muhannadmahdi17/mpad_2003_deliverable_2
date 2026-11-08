**Date**<br>
**Course Code & Course Name**<br>
**Student's First Name & Last Name**<br>
**Presented to Jean-Sébastien Marier**<br>

# Deliverable 2: Exploratory Data Analysis (EDA)
# 1. Getting Data

## Short Brief
For this data on financial security, I decided to do a quick analysis of the percentage of people who live in Ottawa-Gatineau. I wanted to see what percentage of those people answered (1) “very easy or easy” to the question, “In the past 12 months—how difficult or easy was it for your household to meet its financial needs in terms of transportation—housing- food- clothing and other necessary expenditures?” 

## Data Link
 https://open.ottawa.ca/datasets/7dc44d40bbaa4a85a6123a9c825b0994_0/explore

## Importing Data:
I firstly clicked on “Files” in the menu bar, then “Import”. A pop-up window appeared and I clicked on “Upload”, then I browsed for my data file on my desktop.

## Screen Capture


## Public Link to m Google Sheets
https://docs.google.com/spreadsheets/d/1UtVkUDePxuuj5qoNmi4nnKvAze5fXYie_CfPQqkrhag/edit?usp=sharing

## General Observation
there are 18 columns and 385 rows in the data set.
Although the data appears almost organized and consistent, it requires some cleaning to enhance its simplicity, precision, and overall quality.

## Specific Observations
Column A displays the dates of data collection, which span from 2020 to 2024.
Column B reveals the geographical location, indicating that all data pertains to the Ottawa-Gatineau region.
Column C represents the question in both English and French.
Column D shows the answer response to the question, which varies between 1 and 3.
1 - is very easy or easy. 
2 - neither difficult nor easy. 
3- is very difficult or difficult.\
## Surprise
  What surprised me when I looked at the data was columns H and I. I didn’t understand what they represented, since the title for them was F95ucl, which made no sense to me!


## Questions
does subgroup column F really matter for the dataset ?
Column M in the Object doesn’t seem necessary in the data set because it only counts the numbers in the column without providing any additional information.  


![](import-screen-capture.png)<br>
*Figure 1: The "Import file" prompt on Google Sheets.*


## 2. Understanding Data

### 2.1. VIMO Analysis

Use three hashtag symbols (`###`) to create a level 3 heading like this one. Please follow this template when it comes to level 1 and level 2 headings. However, you can use level 3 headings as you see fit.

### Validity Analysis
After a quick scan of the data, I kind of started analyzing what could and couldn't be valid in the data set. No actions. I just was scanning and analyzing what should or what I could do and here is the detailed analysis.
First, I noticed that every row appears twice, once in English and once in French. So I only used the 192-English rows, so nothing gets counted twice.

### Column G, Percent_Pourcent. 
All the values were numbers between 0 and 100, and none were missing. I also checked that the three answers for each group added up to 100% in ach year. They all did, give or take 0.1% from rounding. I found six values that stood out from the rest, and all of them were from 2021. For example, only 7.6% of people aged 65 and older said it was hard to pay for their needs. I kept these values because they probably show what really happened in 2021, not mistakes.

### Column J, Data_quality_Qualité_des_données.
At first, this column looked like it had 144 empty cells. But I learned that an empty cell means the number is reliable. The other 48 rows have an “E,” which means “use with caution.” Half of these are from 2021, and most are in the age groups. This is likely because fewer people were surveyed in each age group.


### Columns H & I , F95lcl & F95ucl. 
These columns show the range where the true value probably falls. Every percentage was inside its range, and nothing was missing. But some ranges were very wide. For people aged 35 to 44 in 2021, the range was 25 points wide. This means small differences between groups may not be real.

I also found two small problems. The “Group” and “Subgroup” column names are switched, and commas in the text were replaced with hyphens.

Overall, the data is complete and makes sense. However, it is less exact for small groups and for 2021. I will keep this in mind when I study the results.

Support your claims by citing relevant sources. Please follow [APA guidelines for in-text citations](https://apastyle.apa.org/style-grammar-guidelines/citations).

**For example:**

As seen in Bounegru & Gray (2011), a data visualization should be clear...

### 2.2. Cleaning Data

I cleaned my data with three methods. First, I froze the header row and made it bold so it stays visible when I scroll. Second, I deleted two columns I didn’t need: ObjectId (column M) and Notes_Remarques, which only repeats the “E” flag. Finally, I swapped the Group and Subgroup values because they were in the wrong columns, and I centered the Year column.

"insert the picture of the screen shot "

### 2.3. Analyzing Data

 

I chose Year, Response, and Subgroup because together they show who is struggling and how this changed over time. Overall financial difficulty stood out: it almost doubled from 16.3% in 2021 to 29.4% in 2024. Difficulty rose for every group, especially people in their late thirties and early forties (19.2% to 37.5%) and people with a disability (20.2% to 37.2%), though some peaked in 2023.

**This section should include a screen capture of your pivot table, like so:**

![](pivot-table-screen-capture.png)<br>
*Figure 2: This pivot table shows...*

**This section should also include a screen capture of your exploratory chart, like so:**

![](chart-screen-capture.png)<br>
*Figure 3: This exploratory chart shows...*

## 3. Delivering Data

I am interested in exploring the rapid increase in financial distress experienced by Ottawa residents. According to the latest statistics, the percentage of people struggling to make ends meet almost doubled, rising from 16.3% in 2021 to a staggering 29.4% in 2024. The hardest hit groups were individuals in their late thirties and early forties, as well as those living with a disability. This reflects a national trend: financial difficulties across Canada roughly doubled between 2021 and 2025 (Pinault & Foran, 2026).

In order to tell this tale, I must first unravel the underlying causes. Statistics on rental rates, food costs, and salaries in Ottawa would reveal the factors at play. I would also want newer Ottawa data and larger samples for the age groups, since many of those results are flagged “use with caution.”

I am considering conducting an interview with Rachael Wilson, the CEO of the Ottawa Food Bank. The organization’s network saw a staggering 101% increase in visits in the 2024–2025 fiscal year, reaching an impressive total of 588,866 visits. I would also like to talk to Ottawa Public Health, a disability advocacy group, as well as parents in their thirties and forties who are grappling with the challenges of housing and childcare costs. CTV News recently reported that seniors and two-parent families are turning to the food bank for assistance in greater numbers (Raymond, 2025).

## 4. References

4. References

City of Ottawa. (2026). Financial security [Data set]. Open Ottawa. https://open.ottawa.ca/maps/7dc44d40bbaa4a85a6123a9c825b0994

Ottawa Food Bank. (2025). Year in review 2024–2025. https://www.ottawafoodbank.ca/year-in-review-2024-2025/

Pinault, L., & Foran, H. (2026, April 9). Stretching the loonie: A time series analysis of financial difficulty and quality of life. Insights on Canadian Society. Statistics Canada. https://www150.statcan.gc.ca/pub/75-006-x/2026002/article/00002-eng.htm

Raymond, T. (2025, November 14). Two-parent families, seniors increasingly turning to Ottawa Food Bank: Report. CTV News. https://www.ctvnews.ca/ottawa/article/two-parent-families-seniors-increasingly-turning-to-ottawa-food-bank-report/

Statistics Canada. (2020). Data accuracy and validation: Methods to ensure the quality of data [Video]. https://www.statcan.gc.ca/en/wtc/data-literacy/catalogue/892000062020008

Statistics Canada. (2022, August 2). Statistically speaking: E does not always stand for excellent. StatCan Plus. https://www.statcan.gc.ca/o1/en/plus/1501-statistically-speaking-e-does-not-always-stand-excellent

**Here's an example:**

Bounegru, L., & Gray, J. (Eds.). (2021). *The Data Journalism Handbook 2: Towards A Critical Data Practice*. Amsterdam University Press. [https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153](https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153)
