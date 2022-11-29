# Capstone_Project_II
Predicting the % of 12th graders in CA high schools who are UC/CSU-ready

# Summary
In part II of the capstone project, I attempted to predict the percentage of students from each California high school who are UC/CSU-ready. The features I looked into 
were: the city the public school is in, public school type, percent of students in the school who are eligible for free/reduced-priced meals, average employment type of 
teachers at the school, whether the school has UC/CSU-approved classes, whether or not the classes in a school is a core academic class under No Child Left Behind 
(NCLB), suspension rate of the school during the 2016-2017 school year, chronic absenteeism rate, and percentage of students in school who are English language learners 
(ELL).

Because the data used were spread out into different datasets, the first part of this assignment (section 2) was devoted to cleaning the data from the California's 
Department of Education (CDE) website and merging the different datasets into one dataframe. This was a challenging feat for me to accomplish because, as someone who 
does not code on a normal basis, a lot of time was devoted to learning more pandas dataframe manipulation techniques as well as trying to match all the data from 
separate datasets into one dataframe. There were cases where some datasets contained information on a set of high schools but other datasets contained information on
another set of high schools that may or may not be in the first set. Therefore, it was crucial to only work with data that incorporated a common set of high schools.

I fitted a linear regression model and a voter regressor ensemble model to this dataframe.

# Conclusion and findings
From this project, we found a few important correlations:

1) As the percentage of students who are eligible for free/reduced-priced meals increases, the percentage of students who are English language learners tends to increase.

2) As the number of classes in a school that are UC/CSU-approved increases, the percentage of students in the school who are UC/CSU-ready tends to increase.

3) As the percentage of 12th grade students who are English language learners at a school increases, the rate of chronic absenteeism tends to increase.

4) As the rate of chronic absenteeism increases, the percentage of students who are UC/CSU-ready tends to decrease.

Additionally, we found that only using the linear regression model results in a model accuracy of 48% while using the voter regressor ensemble model increases the 
accuracy of the model to 76%. The most important features in predicting the percentage of students who are UC/CSU-ready include the type of virtual classroom, whether
the classes in a school are UC/CSU approved, whether the school is a charter school or not, the chronic absenteeism rate, and the suspension rate.

# Recommendations
From our findings, we saw that as the number of classes in a school that are UC/CSU-approved increases, the percentage of students in school who are UC/CSU-ready tends
to increases as well. Therefore, one way to increase the number of students who are UC/CSU-ready is by diverting funds towards:

1) training teachers to teach UC/CSU-approved classes AND

2) resources that compliment a UC/CSU-approved class such as textbooks/access to online academic journals and science laboratory chemicals/instruments.

We also saw that as the rate of chronic absenteeism increases, the percentage of students who are UC/CSU-ready tends to decrease. Further, we see that the rate of 
chronic absenteeism is directly correlated with the percentage of 12th grade students who are English language learners. In other words, from my experience as a high 
school teacher, many of my students who were English language learners were absent often because the language barrier makes it unmotivating to attend class. To solve 
this issue, the hiring of bilingual teachers would be beneficial in helping English language learners staying motivated in class and ensuring that they do not fall 
behind.
