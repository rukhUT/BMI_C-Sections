# BMI_C-Sections
BMI linearly predicts probability of c-section with an R-squared of 0.999!

This project explores CDC birth data to investigate variables that predict risk factors for delivery via Caesarian section.

Data:
* 3.8M births
* 2018 only
* US only

BMI:
* BMI stands for body mass index. It's a ratio of weight to height. Higher BMI means someone is heavier, with very high BMIs meaning obese.
* Anything less than 18.5 is considered underweight and poses underweight health risks.
* Anything greater than 25 is considered overweight and poses overweight health risks.
* Anything greater than 30 is considered obese and poses overweight health risks.
* Anything greater than 40 is considered obese class III and poses significant health risks.
* BMI of 18.5 for a relatively average American woman's height of 5'5 is 111 lbs.
* BMI of 49.9 for a relatively average American woman's height of 5'5 is 300 lbs.
* 96% of births in the data were delivered by mothers with a BMI between 18.5-49.9.

Findings:
* For women with a BMI between 18.5-49.9, BMI linearly predicted the rates of C-section so accurately, it looks like a Google image of a regression.
* The chances of C-section delivery are 1.17 times the mother's BMI. So of women with a BMI of 20, about 23% of them delivered via C-section.
* This was with an OLS R-squared of 0.999!
* Even including all of the birth data including extremely low BMIs below 18.5 and extremely high BMIs above 49.9, the OLS R-squared is still 0.967.

* However like with all health risks, at the extremes there is much more variance in C-section rates due to exacerbating health factors.

  See LMBMIVRATE.png for a scatter plot with the regression line. Interestingly, the linear prediciton stays stable even at class I, II, and III obesity as well as 10 BMI beyond that.

  See LMBMIVRATE_scatter.png for a scatter plot including extreme BMI ranges, and note the increased rates of C-sections at the extremes that are not predicted well by a linear model.

  -Rukh
