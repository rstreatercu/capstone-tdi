# College/University COVID-19 Resilience

In this project, I aim to investigate the resilience of various colleges and universities in the face of COVID-19, using data from the Integrated Postsecondary Education Data System (IPEDS). I wish to determine the role that financial aid, student services staff funding and salary, electronic funding, and more played in determining the effect of COVID-19 on Fall 2020 enrollments at various universities in the United States. Ultimately, I hope to answer the question: how can universities and colleges retain enrollment in the face of pandemics? Since many schools' Fall 2020 enrollment data has only recently been released to the public, there have not been any large-scale investigations on how schools maintained enrollment during the pandemic. I believe that this investigation could help universities prepare for future pandemics and disasters so that they can maintain their enrollment and income without the need for staff/faculty layoffs.

As a preliminary exploration, I downloaded and analyzed shared American university data from IPEDS. To judge enrollment resilience, I used Pandas in a Jupyter Notebook to explore colleges with enough enrollment data (>200 students) to project expected 2020 enrollment. Since many universities have extremely bumpy enrollment due to external factors (see Figure 1 in capstone.ipynb), I used the last n points up to 2019 for which the r^2 value was greater than 0.85 to make a linear trendline. I compared the forecasted 2020 enrollment value with the true enrollment value as a fraction to determine enrollment resilience. I then investigated the correlations between enrollment resilience and other data columns in the set. I was surprised to see that some factors such as staff numbers, admissions rates, and financial aid did not have strong correlations with enrollment resilience. However, I found that budgetary spending on research, institution, and student services and admissions yield were positively correlated with enrollment resistance. 

## Asset 1
Figure 'spending.png'. The plot shows some positive correlations between university spending in student services, institutional support, and research. For tens of millions of dollars, there is a positive increase towards zero, implying that spending  improves pandemic resilience. Beyond 100 million dollars, there is very little trend in resilience, implying that spending is only helpful up to the 100 million dollar point. The fact that institutional size category and hospital spending do not correlate with pandemic resiliency (0.007531) and (0.069442) implies that this effect is independent from general spending and enrollment.

## Asset 2
Figure 'yield.png'. The plot shows some positive correlation between admissions yield (percentage of admitted students  attending) and pandemic resiliency. Since admissions rates were not correlated with resiliency (0.026648 in 2020), there may be some other reason for the correlation, such as ability to attract students with a positive campus atmosphere or location. I would like to investigate these variables in the future.