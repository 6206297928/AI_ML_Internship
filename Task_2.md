*Identify patterns, trends, or anomalies in the data.
1. Survival Patterns
Class matters:

Pclass and Survived are negatively correlated (–0.34).

1st class passengers had much higher survival rates compared to 3rd class.

Likely due to better access to lifeboats and priority evacuation.

Fare influences survival:

Positive correlation (+0.26) with Survived.

Higher-paying passengers had better chances of survival — often 1st class.

Slight edge for family travelers:

Parch and SibSp have weak positive correlation with Survived.
People traveling with family had a slightly higher chance of surviving, possibly due to support during the chaos.

2.2. Age Distribution & Trends
Wide spread of age:

From infants to elderly (0.42 to ~80 years).

Median around 28 years.

Outliers in age:

Boxplots often show some extremely old passengers as outliers.

You might see a few children with very young ages (<1 year).

Younger passengers may have slightly higher survival, but correlation is weak (–0.08).

3.Fare Distribution & Outliers
Highly right-skewed (from histograms):

Most passengers paid less than $50, but some paid over $500 (luxury cabins).

Boxplots show strong outliers in fare:

These high-paying passengers likely in 1st class.

4.SibSp and Parch Patterns
Most passengers traveled alone:

SibSp = 0 and Parch = 0 were common.

People with 1 or 2 family members had better survival odds.

Large families (SibSp > 3 or Parch > 2) might have had lower survival, possibly due to difficulty evacuating as a group.

5. Correlation Highlights
   Pair	                Corr	                 Insight
Pclass & Fare	      –0.55	                Higher class → Higher fare
Pclass & Age	      –0.37	                3rd class had younger people
SibSp & Parch	      +0.41	                Family travelers often had both
Survived & Pclass	  –0.34	                1st class more likely to survive
Survived & Fare	      +0.26	                Richer passengers had better survival chances

6. Anomalies
Fare Outliers: Some passengers paid > $500 — extreme compared to most others.

Age Outliers: Passengers aged 70–80 or babies under 1 year are unusual.

PassengerId: Just a sequence — not useful for modeling or analysis.

Missing Data (not shown in your image but common):

Age often has missing values (around 20% in original dataset).

Q:Make basic feature-level inferences from visuals.

Feature	                                           Key Inference
Survived	                               More passengers died; class, gender, and fare influence survival
Pclass	                                   1st class had highest survival; strong predictor
Sex	                                       Females survived more than males
Age	                                       Younger passengers had slightly better survival
Fare	                                   Higher fare → more likely to survive; right-skewed
SibSp	                                   1–2 siblings/spouses slightly boost survival; large groups hurt it
Parch	                                   Small families better; large ones hurt
PassengerId	                               No analytical value