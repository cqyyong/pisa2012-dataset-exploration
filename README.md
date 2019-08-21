# PISA 2012 Dataset Exploration

## Introduction
This project explores the Programme for International Student Assessment (PISA) dataset. <https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisa2012.csv.zip>

PISA assesses the extent to which 15-year-old students have acquired key knowledge and skills that are essential for full participation in modern societies. The assessment, which focuses on reading, mathematics, science and problem-solving, does not just ascertain whether students can reproduce what they have learned; it also examines how well they can extrapolate from what they have learned and apply that knowledge in unfamiliar settings, both in and outside of school.

## Dataset
There are 485,490 students covered in the dataset with 635 features. 64 countries are represented. Some interesting features include attributes such as country, gender, parents' academic qualifications and the students' maths score and attitudes towards maths (e.g. math interest, self concept, anxiety, work ethic and behaviour). The features are a mix of either categorical/ordinal in nature (such as parents' academic qualifications and attitudes towards maths), or numeric in nature (such as maths score and class periods per week).

## Summary of Findings
1. **Mean Scores.** The mean maths, reading and science scores are normally distributed overall, with values of 469, 472 and 475 respectively.
2. **Gender.** The proportion of male and female students are quite balanced at 49.52% and 50.48% respectively.
3. **Distribution of Maths Score by Gender.** Interestingly, it can be observed that the math scores for males and females looks very similar - normally distributed, with similar means (roughly between 400 to 450) and similar range (slightly below 200 to slightly above 800). Overall there does not look to be any significant difference in the math score between the genders, with the small exception of a higher peak for females at the mean (i.e. more female students having mean scores for maths compared to male students)
4. **Country.** The top 3 countries with the highest mean maths scores are China-Shanghai, Singapore and Hong Kong-China. The bottom 3 countries with the lowest mean maths scores are Peru, Indonesia and Qatar. Interstingly hey are all non-OECD countries. In terms of maths scores, for OECD countries, the math score looks normally distributed with a mean score around 500, with a peak of more than 20000 students achieving the mean score. For non-OECD countries, the math score looks slightly right-skewed (i.e. more students obtain lower scores). Compared with OECD countries, the mean math score for non-OECD countries looks lower at about 400, with a lower peak of about 15000 students.
5. **Educational Qualifications of Parents.** In general, the higher the educational qualification of the parents, the better the mean scores in maths, reading and science for the students.
6. **Family Wealth**
    - **Possessions (own room).** The majority of the students are in possession of their own room. In general, students with possession of their own room tend to have a better mean maths score, but the difference is not significantly large compared to students without possession of their own room.
    - **Possessions (Internet).** The majority of the students are in possession of Internet. In general, students with possession of Internet tend to have a better mean maths score (> 50 points) compared to students without possession of their own room.
    - **Cellular Phones.** The majority of the families have three or more cell phones, and the number of students for this category alone is much more than that combined for students with zero, one or two cell phones. This could be due to the ubiquitous nature of the modern cell phone. In general, students in families with more cell phones tend to have a better mean maths score.
    - **Televisions.** The majority of the families have three or more TVs. In general, students in families with more TVs tend to have a better mean maths score.
    - **Computers.** The majority of the families have three or more computers, but second in place is 'one computer'. It seems that there are more students with one computer compared with the number of students with two computers. In general, students in families with more computers tend to have a better mean maths score.
    - **Cars.** The majority of the students stay in families with 1 car, followed by 2 cars, zero cars and three or more cars. It seems that in general, students in families with more cars (up to two cars) tend to have a better mean maths score. Interestingly, the students in families with three or more cars do not have a better mean maths score than those students in families with two cars.
    - **Books at Home.** The majority of the students have 26-100 books at home. In general, students with more books at home have a better mean maths score.
7. **Wealth Score.** The distribution of the mean maths score for Liechtenstein is almost totally flat. It is noticed that its wealth distribution is almost flat as well, in sharp comparison with the other countries.
8. **Relationships between Scores for Maths, Reading and Science.** In general, the mean scores for maths, reading and science are all positively correlated strongly with one another. This means that a student who is strong in maths will usually be strong in science and reading as well, and vice versa. There is no significant difference in the trends observed for genders. When plotted on a violinplot, we are able to see that there is a difference in the distribution of the maths scores for OECD and non-OECD countries.
