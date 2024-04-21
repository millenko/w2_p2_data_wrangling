![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# QUEST | Maybe there's a 🦈 in the water

<br>

## Introduction

Welcome to the "Maybe there's a 🦈 in the water" data analysis project. Dive in, bite into it!
<br>
In this project, we will share with you information about global 🦈 attack reports, demonstrate our newly acquired data wrangling and analysis techniques.
<br>
Then, hopefully, you will share with us some admiration for the job well-done, as well as other, constructive feedback.
<br>

For a while, our motivation for the project was to get a passing grade, until we remembered that Ironhack is not that kind of school.
<br>
After that, our motives became less ulterior and more altruistic, which is to determine what and how much have we learned so far, and to continue the learning.
<br>
We hope to be a contributing factor to decrease in the 🦈-related accidents, for the sake of both humans and 🦈.

## Team members
- Deimante Piraityte
- Oğuzhan Şahingöz
- Sophiya Siddiqui
- Milenko Rosić

## Installation & setup
- Fork this repo
- Clone it to your machine

### Required environment
- Jupyter Notebook
- Python is 3.11.5 or higher
- Pandas
- Seaborn
- Matplotlib

## About the dataset
The dataset used in this analysis is [GSAF Incident Log](https://www.sharkattackfile.net/incidentlog.htm).
<br>
The mission of the Global Shark Attack File is to provide current and historical data on 🦈/human interactions for those who seek accurate and meaningful information and verifiable references.
<br>
It is the goal of the Global Shark Attack File to demonstrate and emphasize, through forensic analysis, the significance of 🦈/human interactions in comparison to the myriad dangers that we face in our daily lives.
<br>
[The original dataset](https://www.sharkattackfile.net/spreadsheets/GSAF5.xls) is in .xls Excel file format, loaded into a Jupyter Notebook for analysis in Python.

### Problem statement
🦈 attack reports seem to be increasing over the past years.

### Hypothesis
An escalation in oceanic activities, such as surfing and swimming, will correlate with an increase in 🦈 attacks along coastal regions of the USA.
<br>

## Understanding the data
We used Pandas built-in functions such as describe, head, info, unique, to familiarize ourselves with the data.
<br>
The original dataset consist of 6965 rows over 23 columns.
<br>
Though it was a promising number that the dataset is well-fulfilled, the dataset proved to be rather dirty.

### Formatting
We used Pandas built-in functions to format the data, to reach clarity and needs of our analysis.
<br>

- The column-names had consistent appearance.
- The values had inconsistent appearance with regards to leading and trailing whitespace, use of the capital letters and abbreviations.
  - These have been corrected by stripping the whitespace, and with functions and methods such as : lambda, applymap, title, .replace.
- "Year" column has been converted to integers, with astype method.
- "Sex" column values have been reduced from multiple unique values to 2: M and F.
there are columns which appear almost empty or mostly populated by missing or useless data.

### Data Description
We did data reduction by using methods: isna, dropna, drop, and with threshhold of 21 na values per row.
<br>
From the original 6965 rows, the dataset was reduced to 1592 rows over 13 columns:
- "Date" : The full date of the reported human/🦈 encounter and injury
- "Year" : The year of the reported human/🦈 encounter and injury
- "Type" : The type of the injury
- "Country" : The country where he reported human/🦈 encounter took place
- "State" : State as in part of the country where the reported 🦈/human report took place,
- "Activity" : The activity in which the injured was engaged when the reported encounter took place,
- "Sex" : gender of the injured person,
- "Injury" : nature and description of the outcome of the 🦈/human encounter,
<br>
We've decided towards dropping the remaining columns for they contained too manu null values or values not relevant to our analysis.

### EDA methods
The analysis focuses on the trends of swimming and surfing activities in the USA in relation to shark attacks over time.
<br>
We utilized Python libraries Seaborn and Matplotlib to explore and visually present present the statistical findings.
<br>

#### Statistical Analysis:
- Calculating metrics such as the Pearson correlation coefficient to quantify the relationship between swimming activities and shark attacks.
<br>

#### Visualisation:
- Created visualizations such as bar plot, line plots and scatter plots to illustrate the trends of swimming and surfing activities over the years, as well as their correlation with shark attacks.

### Under the hood
- Data structures used: lists, dictionaries, sets
- Flow control: if-else statements
- Functions: mostly Pandas built-in functions and methods
- 

## Conclusion
Our null hypothesis was that an escalation in oceanic activities, such as surfing and swimming, will correlate with an increase in 🦈 attacks along coastal regions of the USA.
<br>
We fail to reject the null hypothesis.
<br>

### Issues and challenges
We won't say anything new if we say that this project was very challenging.
<br>
It was as challenging as the previous project, and as challenging as the next week's one.
<br>
While this bootcamp is an invaluable opportunity to gain the knowledge we expressly came for, the learning-time ratio is inadequate.
<br>
Without prior background in programming, to some of us the struggle is real, and it takes its physical and mental toll.
<br>
Hopefully, you'll take our broken spirits into consideration while observing for broken codes. <p>&#128148;</p>

### Acknowledgements
- GSAF Field Investigators
- Don Nacho
- Simi
- Pedro (though we're still not sure if that's a real person or AI)

### P.S. : No 🦈 was harmed in creating this analysis.
