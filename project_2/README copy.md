
###### Overview

My second foray into DS covers:

- Basic statistics (distributions, correlations, Hypothesis testing)
- Python programing
- Programmatically interacting with files and directories
- Data Cleaning
- Exploratory data analysis
- Exploratory Visualizations
- Pre-processing
- Feature Engineering
- Modeling
- Inferential Visualizations
- Business Recommendations

Intro: For my second project, I wanted to take a look at which home feature would offset its cost and possibly add value to the home.

I wanted to hone in on a overlooked feature, which homeowners don't see typically, as important to overall valuation. Aside from roof upgrades, kitchens upgrades, finishing out basements and adding bathrooms, I decided on driveways, since values were free off nulls and required just binary assignment. the column only has three driveway type categories, so it made it easier to drill down by Building type, Zoning, Building class etc..

##Data Visualizations on Tableau:

https://public.tableau.com/profile/julian.broche#!/vizhome/AmesIowadata_viz/Dashboard1? publish=yes

##### Problem Statement

I've been hired by Grimes Asphalt & Paving to explore the Ames Iowa dataset, in order to solicit customers within the city limits of Ames, Iowa. Utilizing EDA and a Predictive MODEL that supports an iOS App on the backend and targeted marketing campaign for potential clients.

Hypothesis: Does paving your driveway lead to statistically significant higher valuation overall and offset cost?

Ho : The average difference in SalePrice between Paved and Unpaved Driveways is Zero

Ha : The average difference in SalePrice between Paved and Unpaved Driveways is not Zero

Short answer: Yes, based on EDA but no based on 2 sample T test...coef of SalePrice does show it pays for itself.


##### Qualitative Findings

• Often a driveway is an overlooked feature of a home

• Value is partially determined by the surrounding neighborhood, if your homes driveway is in bad shape and all others are in good shape, your home will have a lower perceived value

• Usually paving a driveway will give you a return of AT LEAST the cost of it being installed

• The average asphalt driveway costs about between $2,924 - $6,549 to install

• While it increases the value of your home, a nice paved driveway might also help sell your home FASTER


##### Quantitative Findings

• Overall Paving Equates to Higher Valuation

• Confidence Intervals for Paved, Partial Paved and Unpaved Driveways by MS_SubClass show statistical significance

• 95% CI for Paved = ~$119k - $161k

• 95% CI for Dirt/Gravel = ~$86k - $131k

• 95% CI for Dirt/Gravel = ~$86k - $131k

• Homes with Paved and Partial Paved driveways on average are higher by 32% and 18% respectively, compared to homes in the
same neighborhood

• Since the 50’s things are looking up for Paved Drive Ways

• Overall quality by Driveway show decent spread between those with driveways

• P_value = 1.55 , we failed to reject our null hypothesis, we need to rethink our question


##### Features

• MSSubClass: The building class

• MSZoning: Identifies the general zoning classification of the sale

• Neighborhood: Physical locations within Ames city limits

• BldgType: Type of dwelling

• OverallQual: Overall material and finish quality

• YearBuilt: Original construction date

• 1stFlrSF: First Floor square feet

• 2ndFlrSF: Second floor square feet

• GarageArea: Size of garage in square feet

• PavedDrive: Paved driveway

• LotArea: Lot size in square feet

• Total_sq: 1stFlrSF + 2ndFlrSF + GarageArea in square feet

• Ratio_lotsq: LotArea / Total_sq in square feet

##### Model Metrics

     Metric  | Value
------------ | -------------
       MSE   | 651624374
       RMSE  | 25,526
       MSLE  | 25,526
       MAE   | 12,799
       R^2   | 0.8873
       Adj R | 0.8693

      Beta ( β) Coefficients
 ---------------- | -------------
Overall_Qual_10   | 651624374
Neighbor_StoneBr  | 25,526
     MS_Zoning_I  | 25,526
     1st_Flr_SF   | 12,799
 Paved_Driveway   | 0.8873


![Image of Residuals](file:///Users/j_b/Desktop/Screen%20Shot%202020-10-09%20at%205.25.36%20PM.png)



########### Conclusion

I recommend property owners to invest into repaving an existing driveway or paving a new one
Data clearly shows it adds value + pays for itself!
