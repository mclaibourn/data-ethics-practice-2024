---
title: "Visualizing Economic Self-Sufficiency: Insights from the Greater Charlottesville Region"
output: 
  html_document: 
    keep_md: true
    toc: true
    toc_float:
      floated: true
      at: left
    toc_depth: 2
date: "2024-05-06"
author:
  - Ander Buckley, Dylan Craig, and Sarah Westphal
---

<style type="text/css">
#TOC {
  position: fixed;
  right: 0px;
  top: 0px;
  width: 200%; /* TOC takes up 25% of the view width */
  height: 25%; /* Full height to make the TOC scrollable down to the bottom */
  overflow-y: auto; /* Enables scrolling within the TOC if the content exceeds the view height */
}

.main-container {
  margin-left: 40px; /* Space from the left side of the screen */
  margin-right: 26%; /* Slightly more than 25% to ensure a gap between the TOC and the main content */
  width: auto; /* Automatically adjust width based on the margins */
  padding-right: 10px; /* Provides a buffer on the right side */
}

body {
  overflow-y: scroll;
  position: relative; /* Ensures that the body is relative to the page */
}
</style>





# Introduction

In 2011, Ridge Shuyler created the Orange Dot Report after [asking](https://www.cvillepodcast.com/2012/01/08/wnrn-wake-up-call-orange-dot-project/) “What does it cost to survive in our community?” He was looking for a better way to assess poverty in the greater Charlottesville area. Survival expenses include food, shelter, clothing, and utilities (Charlottesville Podcast Network, 2012). The [Orange Dot Report](https://www.virginiaequitycenter.org/research/orange-dot-report) seeks to describe the characteristics and conditions of families living in the greater Charlottesville area. While the Orange Dot Report has undergone various updates since its inception, its data sourcing remains centered on the American Community Survey by the U.S. Census. This entails utilizing tables provided by the Census department, which offer summarized data at both county and tract levels. In its latest iteration, the report integrates public-use microdata samples (PUMS), enhancing the accuracy of family income assessments across the region. Leveraging PUMS data allows for more precise estimations of family incomes, enabling comparisons with self-sufficiency benchmarks tailored to different family compositions, including considerations such as the number and ages of children. A limitation of the PUMS data is that it cannot be separated by locality (county) or neighborhood (tract).

The primary focus of this report lies in the economic self-sufficiency standard (SSS), a metric designed to determine the amount of income required by families of specific compositions within a particular locale to sufficiently cover their fundamental expenses without relying on any form of public or private aid (Pearce, 2019). The self-sufficiency standard calculates the cost of housing, child care, food, transportation, health care, miscellaneous items, and taxes/tax credits (Center for Women's Welfare, 2021). This takes Ridge Shuyler’s original idea a step further, considering all the elements a household has to consider to survive. In this report, we focus on the economic SSS for households in the greater Charlottesville area to better understand who is and who is not making a livable wage. Employing the economic self-sufficiency standard offers a more precise gauge of poverty compared to the federal poverty line (FPL). This is due to its consideration of factors such as the age of children, geographical location, and all significant expenses encountered by working adults, rather than solely focusing on food costs (University of Washington, 2024). The self-sufficiency threshold varies depending on the composition of households, considering both children and adults. This threshold is determined by calculating the median across all counties and cities for each combination of adults and children. For instance, the threshold differs between a two-parent household with a preschooler and one with a teenager. We opted for a median economic self-sufficiency threshold due to the constraint of the PUMS data, which cannot be segmented by locality or tract. 

# Insights on Those Below the Economic Self-Sufficiency Standard Threshold

## Number and Percent of Households Below the Economic Self-Sufficiency Standard Threshold

The data sample includes a total of 11,127 households in the greater Charlottesville area. We decided to group the data by household instead of family because not all households include a standard “family” as defined by traditional marriage. For example, the increase of cohabiting same-sex couples in the last decade has encouraged the Census Bureau to explore new ways to describe living arrangements (McFalls, 2023). We also wanted to consider multi-generational households, which grouping by family would not consider. 

There are 8,453 households above the economic SSS threshold and 2,674 below the threshold in the data sample of the greater Charlottesville region. However, after weighting for expected population values in the greater Charlottesville area, we were left with a more accurate figure of 74,839 households above the economic self-sufficiency threshold and 27,343 households below the economic self-sufficiency threshold. This represents more than a quarter of households in the area being below economic self-sufficiency.



![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-3-1.png)<!-- -->![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-3-2.png)<!-- -->

## Racial Composition

Importantly, the distribution of economic self-sufficiency is not equal across all demographics. As seen in the graphs, White households are underrepresented, and Black, Asian, and multi-racial households are overrepresented in the distribution of the households below the economic self-sufficiency threshold. This finding is consistent with Joshi, et al.’s (2022) finding that Black, Hispanic, and immigrant households, are less likely to be economically self-sufficient due to the detrimental impacts of systemic racism, including racial disparities in socioeconomic status such as housing, education, employment, and access to health care and social services. 

Interestingly, Joshi, et al. also found that Asian households are the most likely of any racial demographic to be economically self-sufficient, contradicting the results presented here. While Black households were more overrepresented in the distribution below the economic self-sufficiency threshold than Asian households, the observed economic self-sufficiency of Asian households still goes against national trends. The specific economic self-sufficiency of Asian households should be studied further in the future, as there are likely place-specific factors contributing to their overrepresentation. 

We were unable to identify immigrant households and therefore were unable to examine this demographic’s characteristics. Furthermore, multiraciality and ethnicity were not examined due to the limitations of this study’s capacity and the sheer volume of data, meaning the characteristics of Hispanic and multi-racial households and other ethnicities were not examined. The two findings of Black households being overrepresented and White households being underrepresented below the economic self-sufficiency threshold were the racial distribution characteristics that were consistent with the broader literature, with Asian households deviating from national trends. 


![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-4-1.png)<!-- -->![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-4-2.png)<!-- -->

## Age

We also saw substantial differences in economic SSS across age demographics, as seen in the graph below. The heads of household for families under the economic SSS threshold were more likely to be around age 24, while the heads of household for families above the economic SSS threshold were more likely to be around age 60. This is consistent with poverty data over the last few decades. There have been notable increases in young adult poverty (ages 17-24) since the 1970s, especially ages 17-18. An examination of the literature on this increase shows a deprioritization of young adults for expansions of safety net programs, a labor market that is unfavorable for the average worker, and the early transition of youth in poverty to adulthood (Hawkins, 2019; Kendig et al., 2014). There is a large drop-off of head of household age below the self-sufficiency standard after the age of 24 because as these younger individuals progress in age, develop their skills, and build up their work experience, their capacity to earn money will increase substantially, leading to a notable enhancement in their salary trajectory over the course of their careers (Haan, 2023).


![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-5-1.png)<!-- -->

## Income

Income is an important factor to consider when looking at the economic SSS because it goes back to Shuyler’s original question about what it costs to survive in the greater Charlottesville area. We know what it costs to survive for each household type in each location, but it is important to examine how much income households below the threshold are making, as shown in the graph below. Households below the economic SSS threshold make between $0 and $100,000. While $100,000 is well above the federal poverty line (FPL), these households are likely to include multiple children, increasing the cost of survival for the household. For example, the FPL for a family of 7 in Virginia in 2022 was only $41,910, while the median economic SSS for a family of 7 in the greater Charlottesville region is actually over $100,000 (Virginia Department of Health, 2022). Majority of the households above the threshold are making over $100,000, while the majority of households below the threshold are making under $40,000. 



![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-6-1.png)<!-- -->



When looking at the distribution of household income by sufficiency status, the following graph shows the high income of households above the economic SSS, well above the $100,000 shown in the graph above. There are obvious outliers in the data sample above the economic SSS that are making well above $1,000,000. We also want to note the difference between wealth and income. Poverty and economic SSS are both calculated based on income, which is wages. The graph below is only income, not wealth, which is most likely much higher as families with higher income tend to have higher levels of wealth (Atskea, 2021).  

![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-7-1.png)<!-- -->

## Hours Worked

When considering the number of hours worked per week for these households, we found that the average number of hours worked per week by a household above the threshold was 39, while the average number for households below the threshold was 32. The median number of hours worked per week is the same for households above and below the economic self-sufficiency threshold.

While the average number of hours worked a week are different for heads of household above and below the economic self-sufficiency threshold, this highlights the variation of hours worked per week by heads of household. This could indicate that there are other factors contributing to the number of hours worked, such as the variation in scheduling for hourly workers or the challenges of childcare faced by single-parent households.



![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-8-1.png)<!-- -->

## Critique of the Federal Poverty Line

Income is where we see the greatest discrepancies with the federal poverty line. As shown in the graph below, many households below the economic SSS threshold are making two and three times the federal poverty line threshold. This means in the greater Charlottesville region there are over 10,000 households with income above the FPL that are considered to be not economically self-sufficient. The implications are that these households are not considered to be living in poverty and therefore are not receiving the assistance they should be from the government, nor are they making a livable wage. This represents the need for the continuation of the Equity Center’s progress toward a more fully and equitable thriving region. 

A research center in Virginia called [United for Alice](https://www.unitedforalice.org/household-budgets-mobile/virginia) fights for people in Virginia who are “ALICE: Asset Limited, Income Constrained, Employed — earning more than the Federal Poverty Level, but not enough to afford the basics where they live.” Households categorized as ALICE or living below the economic SSS confront difficult decisions, like choosing between investing in quality child care and meeting rent obligations. These choices carry lasting impacts not just for their own families but for society as a whole (United for ALICE, 202). The minimum wage in Virginia is $12, but with rising rent costs and high costs of quality child care, it is not enough for families to survive (The Commonwealth Institute, 2024). 

ALICE households are also battling food insecurity because most often their income is outside of the 130% of the FPL range to receive Supplemental Nutrition Assistance Program (SNAP) benefits. Rising inflation continues to increase the cost of food, which ALICE families cannot afford (Reznickova, 2023). This continues to show the Federal Poverty Line is not a good measure of poverty and what it means to live and survive in today’s economy. The food assistance offered by the Virginia Department of Social Services is only eligible to those eligible for SNAP. This shows a big gap in how Virginia is taking care of the households who are food insecure, but living above the FPL. 

![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-9-1.png)<!-- -->

## Housing Burden

Because of the disparity with government assistance according to the FPL, we decided to look into the housing burden in the greater Charlottesville area. We found that over 60% of households below the economic self-sufficiency threshold are considered housing-burdened. According to the U.S. Census Bureau, a household is housing-burdened when it is spending 30% or more of its income on housing costs (US Census Bureau, 2022).  However, some argue that this traditional measure of housing burden does not account for the fact that costs of living are variable depending on household composition and location, making economic self-sufficiency a better measure of housing insecurity, as it accounts for variable costs (HUD PD&R 2019). The antiquated use of the traditional ratio measure of housing burden leads to severe underestimations of housing burden in low-income areas. 

Additionally, affordable housing is a major factor impacting poverty, further emphasizing the need for public assistance for those above the FPL and below the economic self-sufficiency threshold (National Low Income Housing Coalition, 2021). As shown in the graphs, over 60% of households are below the economic self-sufficiency threshold when only accounting for household income, with the consideration of public assistance income pushing this to just under 50%, meaning that about 10% of households that are above economic self-sufficiency would not be without public assistance. This is a vital consideration when evaluating housing burden, as public assistance income could cause misrepresentations of the true extent of housing burden. Further, public assistance benefits expirations or policy changes could potentially negatively impact the economic self-sufficiency of these households
 

![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-10-1.png)<!-- -->![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-10-2.png)<!-- -->

## Household Composition

Furthermore, there are disparities by household type. Married households are underrepresented in the distribution of households below economic SSS, likely due to the multiple streams of income and tax breaks associated with marriage. Non-married households, including cohabiting and single-parent households, were overrepresented in the distribution. Particularly, households with single females with children are the most overrepresented of the household types, suggesting that the intersecting systemic inequalities associated with gender and socioeconomic status run true here (Joshi, et al. 2022; Lindhorst Everhardt 2010).

![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-11-1.png)<!-- -->

# A Closer Look at Single-Parent Households

Considering that households with single mothers are the most overrepresented in the distribution of households below the economic self-sufficiency threshold, this study takes a deeper dive into the stories of these households, which appear to experience the greatest socioeconomic disadvantage. self-sufficiency status. 

## Hours Worked

On average, the heads of household for single parent households and non-single parent households work the same number of hours per week, as shown in the graph below. But, we know there is a disparity in their economic self-sufficiency status. The [Single Parent Project](https://www.singleparentproject.org/) is a non-profit specifically for single parent households that are above the Federal Poverty Line, but still below the economic self-sufficiency standard threshold. They operate with the understanding that economic self-sufficiency is built for a two-income or two-parent household world, but that is not the case for every family. One of their main goals, as is often found in the literature, is to help single parents become financially stable through support, resources, and education (Single Parent Project, 2021). 

Single parents have actively begged Congress for changes to the federal poverty line for years. In 2020, Mary Jo Hutchinson gave an [impassioned speech](https://www.youtube.com/watch?v=-ptHavHrDuE) in front of Congress explaining how difficult it is to work full time on a minimum wage salary because working full time puts her family right above the FPL and out of reach of government assistance. She says she is often labeled as lazy and not hard-working, even though she is working full-time to try and make ends meet (Reneau & Staff, 2020). The same is happening to single-parent households in the greater Charlottesville region.

![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-12-1.png)<!-- -->

## Number of Children per Household

Single-parent households on average had more children than non-single-parent households. While it is unclear why this is the case, the greater number of children likely leads to increased household costs and therefore less of an ability to be economically self-sufficient. More importantly, this shows how the number of children varies and should be taken into account when calculating economic SSS, as more children lead to increased household costs. Research shows that children raised in single-parent households are more likely to experience adverse outcomes compared to those from married-parent households (Casey, 2022).


![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-13-1.png)<!-- -->

## Racial Composition

Households of color, specifically households with a Black or Asian American head of household, were disproportionately made up of single-parent households, while households with White heads of household were disproportionately made up of non-single-parent households. While it is unclear why this is the case, this shines light on a possible reason for decreased economic SSS for households of color compared to White households, as single-parent households have less income and face child care barriers. More importantly, this shows that, among single-parent households, households of color are overrepresented and disproportionately affected by the reduced level of income. Research shows that not only are people of color more likely to live in poverty than their White counterparts, but single-parent people of color are more likely to live in poverty than their White counterparts. Additionally, research indicates that single mothers from minority backgrounds are disproportionately affected by poverty and encounter substantial obstacles in accumulating wealth (Kerby, 2012). It is beyond the scope of this project to fully analyze these disparities, but as we look through the literature, we find a lack of analyses of these disparities generally. We especially see a lack of literature on single-parent households above the FPL and below the economic SSS threshold

![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-14-1.png)<!-- -->

## Housing Burden

Single-parent households were also disproportionately housing-burdened compared to non-single-parent households. While the inclusion of public assistance income made housing burden comparable for non-single parent and single-parent households, evaluating housing burden based on household income alone shows much larger disparities, with nearly half of the housing-burdened single-parent households relying on public assistance income. This is likely due to the lower income of single-parent households, leading to less income about housing costs, and therefore a higher rate of housing burden. Furthermore, as shown, public assistance is critical to the housing security of single-parent households.

![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-15-1.png)<!-- -->![](EconomicSelfSufficiency-Final_files/figure-html/unnamed-chunk-15-2.png)<!-- -->

## Conclusion

The stark reality of the data is that there are over 10,000 households in the greater Charlottesville region that are living above the Federal Poverty Line who are not economically self-sufficient. These households are not making a livable wage, but are not eligible to receive assistance from the government. This is disproportionately affecting households where the head of household is a person of color. While this project does show this disparity, more research and analysis is needed on these specific households to better understand their situation and experiences. 

As shown, single-parent households are disproportionately impacted by costs and therefore are overrepresented below the economic SSS scale. Furthermore, households of color are overrepresented among single-parent households, meaning these households experience the most severe impacts of being below economic SSS and facing shelter burden in the greater Charlottesville region. While it is difficult to pinpoint the causes and nuances of this, decreased income is one potential cause based on the scope of this project. Beyond this, it is possible that single-parent households do not have access to as many benefits as non-single-parent households, such as certain tax provisions favoring married households. Another possibility is single parent households could be working lower-wage jobs due to child care needs and the lack of flexibility provided by salaried positions. Overall, it is clear that single-parent households are disadvantaged and require more support to maintain economic SSS. 

Potential policies to address this impact include making benefits and services more accessible to single-parent households. Child care, for example, is a critical area that single mothers struggle to access, meaning they often have to sacrifice income to pay for expensive child care or take off work to take care of their children. Providing child care to all workers, regardless of their job type, is one potential solution. Another potential solution is helping single-parent households build wealth through resources and educational services. The literature shows that reduced incomes frequently restrict their ability to participate in wealth-building endeavors such as pension plans due to limited job benefits and resources. Diminished earnings can impede their capacity to invest and save, crucial strategies for wealth accumulation. Wealth not only influences economic stability but also long-term retirement security (Kerby, 2012). Finally, public assistance programs are integral to the economic self-sufficiency of single-parent households, twice as many of which would be housing burdened and 10% more of which would be below the economic SSS if not for public assistance programs. These programs should be maintained and expanded to support single-parent households, which experience the greatest economic disadvantage.


# References

Atske, S. (2021, July 23). “What’s the difference between income and wealth?” and other common questions about economic concepts. Pew Research Center; Pew Research Center. [Link](https://www.pewresearch.org/decoded/2021/07/23/whats-the-difference-between-income-and-wealth-and-other-common-questions-about-economic-concepts/)

Casey, A. E. (2022, August). Child Well-Being in Single-Parent Families. The Annie E. Casey Foundation. [Link](https://www.aecf.org/blog/child-well-being-in-single-parent-families)

Center for Women's Welfare. (2021, April 28). Methodology - Self-Sufficiency Standard. Self Sufficiency Standard. [Link](https://selfsufficiencystandard.org/the-standard/methodology/)

Charlottesville Podcast Network. (2012, January 8). WNRN Wake-Up Call: Orange Dot Project – Charlottesville Podcasting Network. Cvillepodcast.com. [Link](https://www.cvillepodcast.com/2012/01/08/wnrn-wake-up-call-orange-dot-project/)

Hawkins, J. (2019). The Rise of Young Adult Poverty in the U.S. Berkeley.

Haan, K. (2023, December 6). Average Salary By Age In 2024. Forbes. [Link](https://www.forbes.com/advisor/business/average-salary-by-age/)

HUD PD&R. (2019). Exploring housing costs and shelter poverty. PD&R EDGE [Link](https://www.huduser.gov/portal/pdredge/pdr-edge-featd-article-031819.html)

Joshi, P., Walters, A. N., Noelke, C., & Acevedo-Garcia, D. (2022). Families’ job characteristics and economic self-sufficiency: Differences by income, race-ethnicity, and nativity. The Russell Sage Foundation Journal of the Social Sciences, 8(5), 67–95. doi:10.7758/rsf.2022.8.5.04

Kerby, S. (2012, April 16). Pay Equity and Single Mothers of Color. Center for American Progress; Center for American Progress. [Link](https://www.americanprogress.org/article/pay-equity-and-single-mothers-of-color/)

Kendig, S. M., Mattingly, M. J., & Bianchi, S. M. (2014). Childhood Poverty and the Transition to Adulthood. Family Relations, 63(2), 271–286. [Link](https://doi.org/10.1111/fare.12061)

Lindhorst Everhardt, S. (2010). Experiencing gender, race, and class in real life: How low-income women of color strive for economic self-sufficiency and homeownership. Interactions and Intersections of Gendered Bodies at Work, at Home, and at Play, 189–212. doi:10.1108/s1529-2126(2010)0000014012

McFalls, J. (2023). What’s a Household? What’s a Family? PRB. [Link](https://www.prb.org/resources/whats-a-household-whats-a-family/)

National Low Income Housing Coalition. (2021). The Problem. National Low Income Housing Coalition. [Link](https://nlihc.org/explore-issues/why-we-care/problem#:~:text=Housing%20is%20the%20key%20to,mobility%20in%20the%20United%20States.)

Pearce, D. (2019). Demographic Characteristics of Households Below Economic Self-Sufficiency in Connecticut, 2019. [Link](https://portal.ct.gov/-/media/OHS/CT-Healthcare-Affordability-Index/Self-Sufficiency-Standard/CT2019_Demo_20191017.pdf)

Reznickova, A. (2023, June 26). Why Living Above the Poverty Line Doesn’t Guarantee Food Security. The Equation: Union of Concerned Scientists. [Link](https://blog.ucsusa.org/alice-reznickova/why-living-above-the-poverty-line-doesnt-guarantee-food-security/)

Reneau, A., & Staff, U. (2020, February 2). Single mom perfectly explains to Congress why the U.S. poverty line needs a total rehaul. Upworthy; Upworthy. [Link](https://www.upworthy.com/poverty-line-congress-rp3)

Single Parent Project. (2021). The Single Parent Project. The Single Parent Project. [Link](https://www.singleparentproject.org/)

The Commonwealth Institute. (2024, January 16). $12 is Not Enough – Virginia Policymakers Must Act on the Minimum Wage - The Commonwealth Institute. The Commonwealth Institute. [Link](https://thecommonwealthinstitute.org/research/12-is-not-enough-virginia-policymakers-must-act-on-the-minimum-wage/)

United for ALICE. (2021). Virginia | UnitedForALICE. Unitedforalice.org. [Link](https://www.unitedforalice.org/household-budgets-mobile/virginia)

University of Washington. (2024). Washington.edu. [Link](https://depts.washington.edu/selfsuff/standard.html#:~:text=Since%20its%20creation%2C%20the%20FPL,of%20children%2C%20nor%20by%20place.&text=The%20Self%2DSufficiency%20Standard%20is,working%20adults%2C%20not%20just%20food.)

US Census Bureau. (2022, December 8). Renters More Likely Than Homeowners to Spend More Than 30% of Income on Housing in Almost All Counties. Census.gov. [Link](https://www.census.gov/library/stories/2022/12/housing-costs-burden.html)

Virginia Department of Health. (2022). FY 2022: Income Requirements by Federal Poverty Level (FPL). [Link](https://www.vdh.virginia.gov/content/uploads/sites/10/2022/02/FY-2022FPL_500NVM.pdf)
