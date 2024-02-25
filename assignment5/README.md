# PISA 2012 Dataset Exploration
## by Daniel Stenberg

## Dataset

PISA is a survey of students' skills and knowledge as they approach the end of compulsory education. This survey examines

* how well students have learned the school curriculum,
* how well prepared they are for life beyond school.

Around 510,000 students in 65 economies took part in the PISA 2012 assessment of reading, mathematics and science. Of those economies, 44 took part in an assessment of creative problem solving and 18 in an assessment of financial literacy.

The list of variables in the dataset can be found here: https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisadict2012.csv&sa=D&ust=1554482573645000

As can be seen in this variable list, there are hundreds of variables in the dataset. Too simplify data import and handling, most of these will immediately be excluded.

The dataset that this exploration will work with will consist of variables relating to:

* Nationality
* Educational levels of each parent (mother and father) as defined by the ISCED levels (0-6)
* PISA scores for math, reading and science

### ISCED Level	Description
| Level | Descriptions |
| ---- | :---------------- |
| 0 | Early childhood education; no education |
| 1 | Primary education |
| 2C-2A | Lower-secondary education (Second stage of basic education) |
| 3C | Upper-secondary education: programmes designed to lead directly to labour market, not to ISCED 5A or 5B (e.g. Apprenticeship, Secondary technical school) |
| 3B | Upper-secondary education: programmes designed to provide direct access to ISCED 5B (e.g. Vocational training) |
| 3A | Upper-secondary education: programmes designed to provide direct access to ISCED 5A (e.g. Higher general secondary/Higher technical secondary school) |
| 4B | Post-secondary non-tertiary education not giving access to level 5 (primarily designed for direct labour market entry, e.g. Schools for medical services, Schools for nursing) |
| 4A | Post-secondary non-tertiary education programmes that prepare for entry to ISCED 5 (e.g. follow-up courses, language schools) |
| 5B | First stage of tertiary education (not leading directly to an advanced research qualification; e.g. Higher technical school, polytechnic) |
| 5A | Bachelor’s, Master’s or equivalent level |
| 6 | Doctoral or equivalent level |

Source: https://ec.europa.eu/eurostat/documents/1978984/6037342/ISCED-EN.pdf

### PISA Scores
PISA scores do not have a substantive meaning as they are not physical units, such as metres or grams. Instead, they are
set in relation to the variation in results observed across all test participants. There is theoretically no minimum or maximum
score in PISA; rather, the results are scaled to fit approximately normal distributions, with means around 500 score points and
standard deviations around 100 score points. In statistical terms, a one-point difference on the PISA scale therefore corresponds to an effect size (Cohen's d) of 0.01; and a 10-point difference to an effect size of 0.10.

Source: https://www.oecd-ilibrary.org/docserver/35665b60-en.pdf?expires=1660135670&id=id&accname=guest&checksum=9EFA6E60B481DFF9E2315DD4D4CA1302


## Summary of Findings

Univariate, bivariate and multivariate analysis were conducted with appropriate visualizations.

### PISA Scores Distribution and Correlation
The distribution of PISA scores in different subjects (math, science, reading) were analyzed where it was found that they are normally distributed, which could be expected from PISA definitions.

Correlation of subject scores with each other was also analyzed where it was found that high scores in each subject often correlate positively with scores in other subjects.

### Student Nationalities
An overview of the students' nationalities was constructed where Mexico had the most study participants and Liechtenstein the least.

### Educational Levels of Parents
It was shown that ISCED level 5 was the most common education level of parents. Some differences between mothers and fathers were noted. On average mothers have slightly higher educational levels than fathers. It was surprising to see how many level 0 parents there were in the dataset. This could, however, look differently in different countries.

### Correlation of Parent Educational Levels and PISA scores
It was shown that the highest PISA scores coincide with a mother with ISCED level 5. This indicates that the mothers have a higher influence on their childrens PISA scores than the fathers.

Interestingly, the lowest score is identifed for mothers with ISCED level 1 and father ISCED level 6.

It was also shown that level 6 ISCED parents is not necessarily correlated with high PISA scores as the average score was slightly lower and with a high variance.

It is also curious that the median PISA score for level 0 parents is higher than for level 1 parents.

## Key Insights for Presentation
The presentation will be focused on the parents educational level, differences in them and their correlation with student PISA scores.