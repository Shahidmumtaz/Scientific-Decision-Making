# Scientific-Decision-Making
Scientific Decision Making


Part One – Hypothesis Test

1.	Question: 
	Should I invest in a biotech or software startup?

2.	H0: null hypothesis

	H0: 50% of biotech or software startups have received equal to $18.7M funding.

3.	Ha: alternative hypothesis
	Ha: Above 50% of biotech or software startups have received above $18.7M funding.

4.	Test statistic: (in terms of a mean or a proportion) 

	Based on calculation of descriptive statistics of startups data from Kaggle.com, the mean funding for startups in all industries is $18.7M.  To reject the null I need to calculate the Test Statistics and also find the median value for each startup.

	So the Test Statistics for biotech show that (TS=(50.7-18.7)/8.3) the sample is 3.9 errors away from the mean.

	The Test Statistics for software show that (TS=(30.6-18.7)/3.5) the sample is 3.4 errors away from the mean.

5.	Table: the downside risk of the false positive and false negative errors, and alpha (critical p-value) and measures to mitigate Type II errors.
Error Mitigation
Error Type	Downside / risk of this error	Current parameters
Type I (false positive)	(e.g. H0 is that a market does not exist. Ha is that a market does exist. Risk is that we may conclude from our experiment that a market exists when for our product when it doesn’t.)
	 (record alpha here)

α = 0.05
Type II (false negative)	(e.g. H0 is a potential client is not a good lead. Ha is that they are a good lead. Risk is that we may omit a large number of potential clients from a contact list despite the fact that they are good leads.)
	(indicate how you will mitigate Type II errors here) 

I will take a larger sample size to mitigate type ii error.  I have taken a sample size of 34 startups for biotech and 68 startups for software to ensure I mitigate the risk of reaching a type ii error.

 
Part Two – Test, Analyze, and Conclude

Restated the null and alternative hypotheses mathematically. 

1.	H0: (state your null hypothesis mathematically)
2.	Ha: (state your alternative hypothesis mathematically)


	To decide to invest in a biotech or software startup,  I need to find out if based on historical data, more than half or 50% of biotech or software startups received more than $18.7M (average funding for all industries) funding from investors or angels since their establishment with at least 95% confidence level.

H0: 50% received funding = $18.7M

Ha: > 50% received funding > $18.7M


3.	p-value calculated: (written as a decimal; for very small numbers used scientific   or engineering notation; e.g. 0.00000035 should be written 3.5 E -7)

	I used “Test for Mean” separately for both startups and also “Test for 2 Means (Ind)”. The p-values from separate Test for Means show:

p-value for biotech: 

The p-value of a 1-tail-right is 0.0002 and the p-value for 2-tailed is 0.0005.
Conversely, the p-value for 1-tail-left is 0.999 failing to reject the null.

p-value for software:

The p-value of a 1-tail-right is 0.0005 and the p-value for 2-tailed is 0.001.
However, the p-value for 1-tail-left is 0.999 which fails to reject the null.

Based on the “Test for 2 means (independent)” the p-values are:

By using the T.DIST Function the p-value of the left-tail is 0.56, right-tail is 0.44 and 2-tailed is 0.88.
By using the TTEST Function the p-value for a right or left tail is 0.015 and
The p-value for a 2-tailed test is 0.03.

4.	Were you able to reject the null? (yes / no)
	The above p-values “1-tial-right and 2-tailed” from “Test for Mean” for both biotech and software are smaller than alpha.  In addition, the TTEST p-values from “Test for 2 Means (ind)” are smaller than the alpha (0.05), therefore, I can reject the null.

5.	What conclusion can you draw about the original question?

	Based on the p-values from “Test for Mean” and the TTEST Function which assumes the null hypothesis is =0, I can reject the null as the p-values are smaller than alpha.

	The above tests only answered half of my question.  The Test for Means and TTEST answered that by rejecting the null hypothesis, I can see that both startups have received more than the average industry funding ($18.7M). However, to fully answer my original question, I needed to also calculate the median value for both startups to find out if above 50% received more than the average funding.  The median values show that more than 50% of startups in both biotech and software received higher than $18.7M funding. Although, this analysis tells me that I can invest in either one of the startups, I need to compare other factors, like the funding rounds, success or failure and ranking into top 500 to make a better decision.

6.	What unexpected information, if any, did hypothesis testing reveal about your original question?

	Although, the means of both biotech ($50.7M) and software ($30.6M) are higher than the all-average funding of ($18.7M), the T.DIST Function of “Test for 2 means (Ind)” did not reject the null.  

