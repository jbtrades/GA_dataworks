
### Overview

My first foray into DS covers:

- Basic statistics (distributions, correlations)
- Python programming concepts
- Programmatically interacting with files and directories
- Visualizations
- Exploratory data analysis
- Working with Jupyter notebooks to aid development and metric reporting

For my first project, I'm going to take a look at aggregate SAT/ACT participation rates in the United States. I'll seek to identify trends in the data and combine my data analysis with outside research to address my problem statement.

Standardized tests have long been a controversial topic for students, administrators, and legislators. Since the 1940's, an increasing number of colleges have been using scores from students' performances on tests like the SAT and the ACT as a measure for college readiness and aptitude

### Problem Statement

I've been hired by a popular college blogging website to analyze if laws, grants and or political motivations that vary state to state may be affecting SAT/ACT participation rates

Does wide dispersion exist between state’s SAT/ ACT participation rates?

Short answer: Yes, based on EDA

### Qualitative Findings

• 16 States ex D.C currently require ACT vs 6 that require SAT

• They differ slightly in terms of what’s tested/formatted but students typically perform the same

• Schools seem to be agnostic towards SAT/ACT

• Only 3 states ex D.C require both; Idaho, Ohio, Tennessee

• If you’re not satisfied with your score on the mandatory test, you can retake after high-school but will cost $$$

• Decisions between SAT/ACT state by state is influenced by political decisions that come from top- down, Fed > State > Local

• States that require the ACT are mostly mid-west, south-east + Hawaii

### Quantitative Findings

• The scale tilts towards the ACT with 34% states having >= 95% participation vs 10% for SAT

• SAT:  mean 38.6% > median 34.0% > mode 3.0% positive skew

• ACT:  mode 100% > mean 59.2% > median 58.5% negative skew

• Although there is clear skew to SAT/ACT, Standard Devs are almost equal

### Conclusion

I recommend digging more into the political associations between parties and SAT/ACT

Data from the Federal Election Commission show that College Board executives have an overwhelming preference for Democratic candidates. The College Board also spends hundreds of thousands of dollars on lobbying, according to the Center for Responsive Politics.

Maybe it’s just a coincidence that states that tend to sway liberal prefer SAT?
