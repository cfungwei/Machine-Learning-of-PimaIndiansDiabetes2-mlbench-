# Machine-Learning-PimaIndiansDiabetes2-mlbench

'PimaIndiansDiabetes2' dataset from mlbench has 768 observations of women of at least 21 years old, of Pima Indian heritage and living near Phoenix,Arizona, on 9 variables : 
   1. pregnant (Number of times pregnant)
   2. glucose	Plasma glucose concentration (glucose tolerance test)
   3. pressure	Diastolic blood pressure (mm Hg)
   4. triceps	Triceps skin fold thickness (mm)
   5. insulin	2-Hour serum insulin (mu U/ml)
   6. mass	Body mass index (weight in kg/(height in m)\^2)
   7. pedigree	Diabetes pedigree function
   8. age	Age (years)
   9. diabetes	Class variable (test for diabetes)
---
Objective of the study is to:
- identify pairs of vairables with high linear correlation 
- correctly identify test set with high accuracy

Data Cleaning
---
Since data consists of numerical variables, we removed observations with NA values. We reduced the data from 786 to 392 observations, consisting of 130 people diagnosed with diabetes and 262 diagnosed without diabetes.

Using the [Pearson correlation coefficient](https://statistics.laerd.com/statistical-guides/pearson-correlation-coefficient-statistical-guide.php), we consider absolute values above 0.5 to be significant. From scatterplot matrix below, there are significant correlation between age and pregnant (0.68), tricep and mass (0.66) and glucose and insulin (0.58).

![scatterplot matrix](https://user-images.githubusercontent.com/97843966/153906081-0dcccc10-f87a-4308-9def-22ca31fa4e9b.png)
