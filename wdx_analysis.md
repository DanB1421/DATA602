# **The effect of worldwide energy consumption on disease mortality and life expectancy from 2000 to 2015**

*Daniel Brilliant*

*Data Science Master's Student, UMBC*

*March 15, 2022*

Human civilization is defined by decisions that produce beneficial and harmful outcomes. One of the most major impacts for humanity that falls into both categories is industrialization. Industrialization has made processes such as manufacturing and transportation much easier than before, but that does not come without a cost. The modified processes produced during the industrial revolution are often fueled by non-renewable resources such as coal, oil, and natural gas, also known as fossil fuels. The aftereffects have caused changes to air quality, water purity, and the ozone layer due to increases in the emission of carbon dioxide (CO<sub>2</sub>).

The effect of CO<sub>2</sub> emissions also showed a direct impact on quality of life, whether this be through breathing in polluted air, prolonged exposure to carcinogens, and access to drinkable water sources. The direct results of these environmental changes can be measured in a variety of statistics, but two that have clear implications on human life are mortality rates from diseases and life expectancies. There are two major questions we can ask about these relationships:
  1. How do CO<sub>2</sub> emissions relate to both mortality rates from disease and life expectancy at birth? 
  2. How does renewable energy usage relate to both mortality rates from disease and life expectancy at birth? 

These can be answered by analyzing the correlation betweren CO<sub>2</sub> emissions and renewable energy usage worldwide in the years 2000 and 2015 to disease mortalities and life expectancy at birth.

## **1. Analysis Strategy and Approach**

- **Data Source:** World Development Explorer ([worlddev.xyz](https://))
- **Countries Analyzed:** Comoros, Denmark, Finland, Hungary, Iceland, Moldova, North Korea (referred to here as Democratic People's Republic of Korea), Sweden, Uruguay, and Zimbabwe
- **Timespan of Data:** 2000-2015
- **Topics & Indicators:**
  - **Environment- Renewable energy consumption (% of total final energy consumption):** the share of renewable energy in the total final energy consumption.
  - **Environment- CO<sub>2</sub> emissions (kt):** emissions of carbon dioxide stemming from the burning of fossil fuels and the manufacture of cement. These can include CO<sub>2</sub> produced during consumption of solid, liquid, and gas fuels and gas flaring.
  - **Health- Cause of death, by non-communicable diseases (% of total):** Cause of death is the share of all deaths at all ages due to underlying causes. Non-communicable diseases include cancer, diabetes mellitus, cardiovascular diseases, digestive diseases, skin diseases, musculoskeletal diseases, and congenital anomalies.
  - **Health- Cause of death, by communicable diseases and maternal, prenatal and nutrition conditions (% of total):** Cause of death is the share of all deaths at all ages due to underlying causes. Communicable diseases and maternal, prenatal, and nutrition conditions include infectious and parasitis diseases, respiratory infections, and nutritional deficiencies such as underweight and stunting.
  - **Health- Life expectancy at birth, total (years):** The number of years a newborn infant would live if prevailing mortality patterns at time of birth remain the same throughout life.

## **2. How do CO<sub>2</sub> emissions relate to life expectancy and mortality rates from communicable and non-communicable disease?**

### **Worldwide CO<sub>2</sub> emission distribution in 2000 and 2015**
![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2000%20CO2%20emissions%20distribution.png)

![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2015%20CO2%20emissions%20distribution.png)

### **Non-communicable disease mortality vs CO<sub>2</sub> emissions in 2000 and 2015, with regression line**
![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2000%20Noncommunicable%20disease%20vs%20CO2.png)

![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2015%20Noncommunicable%20disease%20vs%20CO2.png)

### **Communicable disease mortality vs CO<sub>2</sub> emissions in 2000 and 2015, with regression line**
![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2000%20Communicable%20disease%20vs%20CO2.png)

![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2015%20Communicable%20disease%20vs%20CO2.png)

### **Life expectancy vs CO<sub>2</sub> emissions in 2000 and 2015, with regression line**
![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2000%20Life%20expectancy%20vs%20CO2.png)

![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2015%20Life%20expectancy%20vs%20CO2.png)

- When looking at worldwide distribution of CO<sub>2</sub> emissions in 2000 and 2015, the right skew of countries at the highest emission level increased in 2015 mainly due to the increase of China's emission level. However, the spread of high-emitting countries aside from China decreased in 2015 and less countries were emitting at a high level than in 2000.
- The p-value analysis and correlation in these comparisons had varied outcomes.
  - For the non-communicable disease mortality comparisons, the link to CO<sub>2</sub> emissions was statistically significant in 2000 (p = 0.016) but not in 2015 (p = 0.063). Neither showed a high level of correlation (r = 0.179 in 2000 and r = 0.138 in 2015)
  - For the communicable disease mortality comparisons, the link to CO<sub>2</sub> emissions was statistically significant in 2000 (p = 0.020), but not in 2015 (p = 0.068). Neither showed a high level of correlation (r = -0.173 in 2000 and r = -0.134 in 2015)
  - For the life expectancy comparisons, the link to CO<sub>2</sub> emissions was statistically signficant in 2000 (p = 0.024), but not in 2015 (p = .101). Neither showed a high level of correlation (r = 0.164 in 2000 and r = 0.122 in 2015)
- Overall, the data showed little correlation between CO<sub>2</sub> emissions and disease mortality or life expectancy for either 2000 or 2015. Conversely, the linkage for all comparisons was statistically significant in the 2000 data, but not in the 2015 data.

## **3. Does an increase in renewable energy usage cause significant changes to mortality rates from disease and life expectancy?**

### **Worldwide renewable energy usage distribution in 2000 and 2015**
![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2000%20Renewable%20energy%20usage%20distribution.png)

![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2015%20Renewable%20energy%20usage%20distribution.png)

### **Non-communicable disease mortality vs Renewable energy usage in 2000 and 2015, with regression line**
![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2000%20Noncommunicable%20disease%20vs%20renewable%20energy.png)

![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2015%20Noncommunicable%20disease%20vs%20renewable%20energy.png)

### **Communicable disease mortality vs Renewable energy usage in 2000 and 2015, with regression line**
![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2000%20Communicable%20disease%20vs%20renewable%20energy.png)

![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2015%20Communicable%20disease%20vs%20renewable%20energy.png)

### **Life expectancy vs Renewable energy usage in 2000 and 2015, with regression line**
![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2000%20Life%20expectancy%20vs%20renewable%20energy.png)

![](https://github.com/DanB1421/world_development_explorer_final/blob/1797ebd62c0b6dddd7b7e7ac6eb9f67478053f95/charts/2015%20Life%20expectancy%20vs%20renewable%20energy.png)

- When looking at worldwide distribution of renewable energy usage in 2000 and 2015, a number of countries increased over time significantly. This shows in a more even but still right skewed distribution. Also, the increase occurred more in a shift in the 0%-30% bins more than 40%-100%, which showed a more even grouping outside of the 70%-80% and 100% bins.
- The p-value analysis and correlation in these comparisons had strong connections.
  - For the non-communicable disease mortality comparisons, the link to renewable energy usage was statistically significant in both 2000 and 2015 (p = 0.000 for both). Both showed a moderate negative correlation (r = -0.757 in 2000 and r = -0.666 in 2015)
  - For the communicable disease mortality comparisons, the link to renewable energy usage was statistically significant in both 2000 and 2015 (p = 0.000 for both). Both showed a moderate positive correlation (r = 0.771 in 2000 and r = .713 in 2015)
  - For the life expectancy comparisons, the link to renewable energy usage was statistically signficant in both 2000 and 2015 (p = 0.000 for both). Both showed a moderate negative correlation(r = -0.748 in 2000 and r = -0.636 in 2015)
- Overall, the data was entirely statistically significant in connecting renewable energy usage to disease mortality and life expectancy. The data also signified that countries with higher renewable energy usage somewhat tended to have lower non-communicable disease mortality rates and lower life expectancies, while the opposite was true for communicable disease mortality rates.

## 4. **Conclusions**
- The changes in distribution of CO<sub>2</sub> emissions and renewable energy usage worldwide between 2000 and 2015 showed evident distinctions in analysis
- The difference in CO<sub>2</sub> emissions distribution caused the disease mortality and life expectancy comparisons to be statistically significant in 2000 but not in 2015. This was not true for renewable energy usage distribution, as the change over time did not affect the statistical significance of the disease mortality and life expectancy comparisons.
- The correlation between CO<sub>2</sub> emissions and disease mortalities or life expectancy was not strong in any of the data sets examined.
- The correlation between renewable energy usage was moderately strong in all data sets examined. The results were somewhat surprising.Non-communicable disease mortality and life expectancy were lower in countries with higher renewable energy usage and communicable disease mortality was higher.
- Some anecdotal observations can be made from the overall results. 
  - CO<sub>2</sub> emissions are not an adequate comparative tool to measure the harmful effects of non-renewable resource usage in relation to disease mortality and life expectancy. Better statistics to look at for analysis would likely be either fossil fuel usage or non-renewable resource usage statistics.
  - Renewable energy usage can be instructive in analyzing the disease mortality and life expectancy of a country. However, further analysis should occur on other factors that determine disease mortality and life expectancy. The correlation is not strong enough on its own to use these comparisons, so further research on other environmental and economic factors is necessary.
