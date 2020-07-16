---
title: "Day6"
lastmod: 2020-06-23
date: 2020-06-23
draft: false
---
# Data visuvalization


**Types of Visualization**

1. **Trends** - Lineplot

2. **Distribution** - (Join,KDE,distplot )

3. **Relationship**- (Bar, heatmap, Scatter, Swarm, Reg, lmplot)

Also the visualization varies as univariate, bivariate and multivariate

3 Angles/Aspects of visualization are univariate, Continuous vs Categorical and Linear regression plot


**Trends:**

1. **Lineplot** - Show trends over period of time. sns.lineplot(data=data)
<br>
![Line plot](../Visuvalization/lineplot.png)

**Distribution:**

1. **Distplot** - Histogram distribution of single numerical value

sns.distplot(a=data['a'],label,kde=true/false)

![Dist plot](../Visuvalization/distplot.png)

2. **KDE plot** - Kernel Density plot smooth distribution of single numerical value

![KDE plot](../Visuvalization/KDEplot.png)

3. **Joint plot** -  Two dimensional KDE plot used for both uni and bi-variate

![Joint plot](../Visuvalization/jointplot.png)

**Relationship:**

1. **Barplot** - Bar charts

![Barplot](../Visuvalization/barplot.png)

2. **HeatMap** - Color coded patterns

![HeatMap](../Visuvalization/heatmap.png)

3. **Scatterplot** -Relationship between continuous variables

![Scatterplot](../Visuvalization/scatterplot.png)

4. **Regplot** - Includes regression line in scatter plot

![Regplot](../Visuvalization/regplot.png)

5. **lmplot** - Multiple Regression line if scatter plot contains multiple values

![lmplot](../Visuvalization/lmplot.png)

6. **Swarmplot** - Comparison between continuous and categorical

![Swarmplot](../Visuvalization/swarmplot.png)

**Note: Strip plot is same as swarm plot.**



Note:

1. Jitter=true/false used for scattering the data esp used in strip plot

2. Swarm plot won't overlap each other as strip plot

3. %matplotlib inline to avoid use of plt.show() multiple times

4. sns.set[color_code=True] so have same colors for multiple runs

5. In addition to the above there are Boxplot, Violinplot, Reisdualplot, counplot. pointplot etc.

6. KDE=false will hide the curve and displays only the histograms

7. Barplots displays a line above the bar and it is called confidence level

8. In joint plot we can provide kind values like points,hexagon..etc

9. regplot() performs a simple linear regression model fit and plot. lmplot() combines regplot() and FacetGrid.

10. FacetGrid object takes a dataframe as input and the names of the variables that will form the row, column, or hue dimensions of the grid.
