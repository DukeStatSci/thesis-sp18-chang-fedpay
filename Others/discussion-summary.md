# discussion summary

## Discussion Summary (02/01)

1.	Check whether data include any part-time employees
2.	Conduct PPC
  a.	Method 1 – Blank all for columns with missing data (more sensitive check) 
  b.	Method 2 – Blank all for columns with missing data of interest (yr_1 & yr_10 salary)
 	Plot Distribution of yr_10 vs. yr_1 
 	Compare imputed vs. replicated (split into SES and non-SES) 
3.	Simulation study to evaluate feasibility of logistics regression
	
## Discussion Summary (02/07)

1.	Use method 2 for PPC (check each dataset 20 times and include the rest in appendix) 
2.	Simulation study
  	a.	Generate a logistic regression model based on true data (P(SES = 1) = pi)
	b.	Simulate outcome variable Y based on pi
	c.	Refit logistic regression model based on the new simulated outcome variable Y
	d.	Compare estimated parameter B with the actual one

## Discussion Summary (02/15& 02/16)

1.	Refine the population
	a.	Combine factor for Grade (ask Alex for dealing with special pay plan)
		i.	Combine grade into four bins (1 - 3,4 - 6, 7 - 9, 10 - 12, 13 - 18, Others)
		ii.	For people whose pay plan are non-ES in year 10 and never get promoted, find the baseline levels for year 10 grade, and toss out those sub-population. 
		iii.	Rethink pay_plan & grade
	b.	Toss out Clerical and Technical occupation category  			
	c.	Toss out Hawaiian & Pacific Islander (none of them are promoted) 
	d.	Special occupation (AD) has very high salary distribution, which produces bias for the model
	e.	Toss out people whose pay plan = ES in year 1
2.	Compare the simulated data Beta with actual data

3.	Redefine Estimated Start Year

##Discussion Summary (02/22)

1.	Add variable svsrstat (indicator of supervisor/manager)
	a.	Remove those who got promoted in the first 10 years
	b.	Remove estimated start year as a predictor 
2.	EDA
	a.	Binned plot to check the relationship between percentage of each group who get promoted given independent variable
	b.	Possibility to apply spline to continuous variable
3.	Model fit
	a.	Binned residuals to check model fit
	b.	Hosmer-Lemeshow goodness of fit test

