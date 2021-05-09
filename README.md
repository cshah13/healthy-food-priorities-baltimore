# Analyzing Healthy Food Availability Throughout Baltimore, Maryland

## Abstract

Almost a quarter of Baltimore residents reside in areas which lack access to healthy, affordable food options. If this problem is not addressed, there will continue to be adverse diet related health issues throughout Baltimore. The Baltimore City Health Department has community based interventions in place, such as subsidies for households growing fresh produce and providing vehicular access to households unable to seek food. However, there is still a significant lack of healthy food availability throughout Baltimore. To this end, we propose to expand existing programming within the Baltimore Food Policy Initiative by reevaluating current programs and reallocating resources based on their effectiveness. We also recommend promoting cost-effective solutions, such as increasing urban agriculture and expanding Supplemental Nutrition Assistance Program (SNAP) participating locations as short and long term goals respectively. 

## Background

Researchers at The [Johns Hopkins University Center for a Liveable Future (CLF)](https://clf.jhsph.edu/about-us/news/news-2018/report-food-desert-gets-name-change-response-baltimore-community-feedback) found that 23.5% of residents in Baltimore, Maryland reside in a food desert, which is a location that lacks access to health, affordable food options. Additionally, 28.8% of youth in Baltimore City are obese. The overall healthy status and outcomes related to diets are worse in Baltimore City than the Maryland average—the leading causes of death are cardiovascular disease and diabetes. [The CLF specifically defines food deserts](https://mdfoodsystemmap.org/wp-content/uploads/2013/01/Atlas_CLF-Food-Swamp_final.pdf) as areas where the closest supermarket is more than ¼ mile away, the median household income is below 185% of the federal poverty level, less than 40% of homes do not have vehicles, and supermarkets have low Healthy Food Availability Index (HFAI) scores. Additionally, food swamps exist within food deserts—food swamps are locations where there is greater accessibility to unhealthy foods compared to healthy foods. [The CLF released a report in 2018](https://clf.jhsph.edu/about-us/news/news-2018/report-food-desert-gets-name-change-response-baltimore-community-feedback) stating the term “food deserts” in Baltimore, Maryland was replaced by Healthy Food Priority Areas to avoid the negative connotations associated with the previous term. Since individuals in Healthy Food Priority Areas throughout Baltimore are experiencing poor health outcomes, the CLF suggests increasing accessibility to healthy food options can contribute to a healthier and equitable food environment. 

[The Baltimore City Health Department has a variety of programs](https://health.baltimorecity.gov/programs/food-access) in place to increase food availability through the Baltimarket program, a set of community-based interventions. Within the program, a Virtual Supermarket Program has been implemented to provide grocery delivery services to low income communities that do not have vehicular access to seek healthy food choices. Furthermore, Baltimore Food Justice Forum provides residents with resources to obtain healthy and affordable foods in their respective neighborhoods. These community based efforts are aimed to implement impactful solutions that mitigate food deserts across Baltimore. The Baltimore City Health Department has [combined resources](https://planning.baltimorecity.gov/baltimore-food-policy-initiative) with the Department of Development Corporation, Department of Planning, and Office of Sustainability to create the Food Policy and Planning Division which oversees the Baltimore Food Policy Initiative. This initiative focuses on empowering communities to increase healthy food availability by incentivizing grocery store owners to increase healthy food availability scores and providing subsidies to households growing fresh produce.

Although there are interventions in place, there is more work that needs to be done to increase food availability throughout Baltimore. If this problem is not addressed, there will continue to be detrimental diet related health effects within the population. This analysis analyzes healthy food availability index scores, median household income, and density of fast food outlets throughout Baltimore to guide the direction of the Baltimore City Health Department programs.

## Business Question
What factors impact healthy food availability in Baltimore?

## Data Question
1. How can 2015 Healthy Food Availability Index Scores be organized in four clusters? [View Analysis Here](https://github.com/cshah13/healthy-food-priorities-baltimore/blob/main/Cluster%20Analysis%20HFAI%202015.xlsx)
2. How do HFAI scores compare across Community Statistical Areas in Baltimore City? [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/cshah13/healthy-food-priorities-baltimore/blob/main/Geospatial_Analysis_HFAI_MedHHI.ipynb)
3. How have the Healthy Food Availability Index scores changed from 2012 to 2015? [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/cshah13/healthy-food-priorities-baltimore/blob/main/HFAI_FoodIndexAnalysis.ipynb)
4. How prevalent are fast food establishments throughout Baltimore City? [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/cshah13/healthy-food-priorities-baltimore/blob/main/Fast_Food_Outlet_Density_Graph.ipynb)
5. How does median household income compare with HFAI scores across Community Statistical Areas in Baltimore City? [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/cshah13/healthy-food-priorities-baltimore/blob/main/Geospatial_Analysis_HFAI_MedHHI.ipynb)


## Data Sources
We used data from the Baltimore City Open Data to conduct this analysis
1. [Healthy Food Availability Index Scores](https://data.baltimorecity.gov/datasets/bniajfi::average-healthy-food-availability-index?geometry=-77.045%2C39.192%2C-76.196%2C39.378&selectedAttribute=hfai15)
2. [Fast Food Outlet Density](https://data.baltimorecity.gov/datasets/bniajfi::fast-food-outlet-density-per-1000-residents)
3. [Median Household Income](https://data.baltimorecity.gov/datasets/bniajfi::median-household-income)

## Data Answer
### How can 2015 Healthy Food Availability Index Scores be organized in four clusters? 
We used the Microsoft Office Excel Solver tool to categorize locations throughout Baltimore based on HFAI scores. The HFAI scores indicate the level of healthy and whole foods available in a store—the highest score of 28.5 indicates the healthiest options. The findings show that 57% of Baltimore locations have an HFAI score less than 9.25. This indicates there is an insufficient availability of healthy, nutritious, and whole food options throughout stores in Baltimore. Since HFAI scores are one of the four indicators of Healthy Food Priority Areas, improving the HFAI can be a positive step towards reducing Healthy Food Priority Areas across Baltimore.

### How do HFAI scores compare across Community Statistical Areas in Baltimore City?
We used Python to create a graph showing HFAI scores in Community Statistical Areas in Baltimore City. Overall, statistical areas with similar HFAI appear to be located next to each other. Statistical areas with HFAI scores of 9.2-11.25 appear to be close together and there is a clear grouping of areas in the center of the map. Statistical areas with lower HFAI scores are located towards the borders of Baltimore City and include popular tourist destinations like Inner Harbor. Statistical areas with HFAI scores between 11.25 and 16 are located in close proximity to one another and form a border along the Baltimore waterfront. The sole area with a HFAI score above 16 is located along the upper border of Baltimore City, and is flanked by statistical areas with low HFAI scores. This finding merits future research to identify additional factors that may explain why it has a high HFAI score while its neighbors do not. ![alttext](https://github.com/cshah13/healthy-food-priorities-baltimore/blob/main/HFAI%20Map.png)

### How have the Healthy Food Availability Index scores changed from 2012 to 2015?
The graph shows that 68% of areas in Baltimore had a decline in HFAI scores during the three year time period. We know this is a problem that the Baltimore City Health Department is attempting to address; however, the interventions are not showing improvements. The graph highlights specific locations in Baltimore where HFAI scores increased or decreased to identify areas that need further attention. Areas such as Chinquapin Park/Belvedere, Beechfield/Ten Hills/West Hills, and Loch Raven experienced the greatest declines (between 5-7 points). On the other hand, locations such as Southeastern and Mount Washington/Coldspring experienced the greatest increases (3-5 points (over 4 points). 

### How prevalent are fast food establishments throughout Baltimore City?
The overall densities of fast food outlets per 1000 residents in community statistical areas were below 5 for both 2013 and 2018, however Downtown/Seton Hill had a significantly higher density than other statistical areas during both years. The next highest values were from Madison/East End, however these values were almost 7, which is more than three times less than the values for Downtown/Seton Hill. The fast food outlet densities were greater in 2018 than 2013 for most statistical areas. The findings of this analysis indicate that fast food outlets are fairly prevalent throughout Baltimore City and extremely prevalent in Downtown/Seton Hill. The fast food outlet density for Downtown/Seton Hill decreased marginally from 2013 to 2018, however it is still significantly higher than all other community statistical areas. 

### How does median household income compare with HFAI scores across Community Statistical Areas in Baltimore City? 
The map  shows the median household income of each community statistical area and puts the HFAI scores in context with financial constraints, a possible factor affecting HFAI scores. Overall, higher income areas correspond to higher HFAI scores. The areas with lower HFAI scores somewhat correspond to lower income areas, however areas with median household incomes of $30,000-$45000 have both medium and low HFAI scores. Areas along the waterfront and inner harbor have higher median household incomes, which suggests that other factors may be influencing their low HFAI scores. 

![alttext](https://github.com/cshah13/healthy-food-priorities-baltimore/blob/main/Household%20Income%20Map.png)

## Recommendations
