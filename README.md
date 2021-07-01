<h1>Capstone Project - Workplace Absenteeism</h1>
<h2>1. Introduction</h2>
<p>Absenteeism is the practice of regularly being absent from work. While employers expect employees to miss some days of work, excessive absenteeism can hurt productivity and the company's bottom line. If employers are more aware of the causes of absenteeism, they are likelier to take steps to alleviate the problems. The goal of this project is to determine the most common causes of absenteeism.</p>

<h2>2. Data Collection</h2>
<p>The data comes from the Machine Learning Repository at the University of California, Irvine, updated April 5, 2018. This data set contains 740 records of absenteeism at work from July 2007 to July 2010 at a Brazilian courier company, in 21 columns. This dataset was accessed from [http://archive.ics.uci.edu/ml/datasets/Absenteeism+at+work].</p>

<h2>3. Data Wrangling</h2>
<p>I made binary columns for regression analysis using one-hot encoding for the categorical variables. I also renamed the new columns from the one-hot encoding and made the existing columns easier to understand. I added a new column with the hours absent logarithmically transformed, and replaced the '-inf' values with zeroes.</p>

<h2>4. Inferential Statistics</h2>
<p>First I calculated the percentage of hours missed for each reason for being absent, each month, each day of the week, each season, each education level, and each binary category, such as smoker/non-smoker. I calculated the correlation values between hours missed and transportation expense, commuting distance, service time, age, height, weight, and body mass index (BMI). Transportation expense, service time, age, and weight had very weak correlations. Height had a slightly stronger correlation. Commuting distance and BMI had very weak negative correlations.</p>

<p>Comparing the mean number of hours missed for each season, month, day of the week, education level showed little significance in the differences between the means.</p>

<h2>5. Machine Learning</h2>
<p>The decision tree model is the best of the models I tried because it showed the highest AUC score, of 0.69.</p>

<h2>6. Final Report</h2>
<p>This notebook contains my complete analysis and results.</p>
