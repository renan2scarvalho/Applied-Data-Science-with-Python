# Course Content:
- Describe how machine learning is different than descriptive statistics;
- Explain different approaches for creating predictive models;
- Create and evaluate data clusters;
- Build features that meet analysis needs.

Here we'll analyze the [crimes](https://www.kaggle.com/dbwaller/official-crime-data-sao-paulo-statebrazil-ssp?fbclid=IwAR239ZovM1Zz3lIccXdxTuIHgaPB_G_YkI6G4HIXu4WUQWqC3Jz8Je3fU3o) in the State of São Paulo, Brazil, as well as its [GDP](https://www.seade.gov.br/produtos/pib-anual/). From these datasets we can try to check several things:

- The population increases in the same rate as the GDP?
- Are the GDP and Per Capita GDP similar?

But here we'll perform a t-test to check our hypothesis: 
 
**Hypothesis H1:** when a recession happens, the criminality increases.

If the p_value < 0.01 we reject the null hypothesis (H0), which means that the criminality stays the same, indepedent of recession periods.

Here, makes more sense to analyze the hypothesis with Per Capita GDP, but we'll perform both analysis. Also, ideally, the GDP should be in a monthly basis, not yearly. But due to the lack of data, we'll perform this analysis on a yearly basis.

Let's define recession, recession bottom, and end end of recession, which are only assumptions, as we'll see in the analysis:

- <b>Recession</b>: we consider a recession 2 consecutive years of negative growth, which ends with 2 consecutive years of GDP growth.
- <b>Recession bottom</b>: year with the lowest GDP.

<img align="center" src="https://user-images.githubusercontent.com/63553829/92014715-0c5a3500-ed26-11ea-8dc0-54685f95370b.png">

Here some other definitions must be made. One should use the Real GDP as the parameter for this analysis, since it considers inflation. The GDP Growth Rate present in the table takes the Year of 2010 as a baseline. Here we'll compute the growht based in the yearly changes, not applying this baseline. so the Growth is calculated as follows:

![image](https://user-images.githubusercontent.com/63553829/92014734-167c3380-ed26-11ea-8798-582c946e6a1b.png)

The Growth Rate isn't necessary for this analysis, since we could perform it only with GDP values. However, they are easier to visualize due to smaller dimensions in comparison with GDP.
