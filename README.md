# Evapo-transpiration and Temperature in Camarillo, California

## Using California Irrigation Management Information System (CIMIS)- Eddy Covariance Station

Final Project - EDS 222 Statistic For Environmental Data Science

# Hypothesis:

1)  State your hypothesis for your final project. Using this week's wildfire lab as an example, your hypothesis could be "The number of wildfires increases with vapor pressure deficit." That's an example of a scientific hypothesis. To state the equivalent statistical hypothesis, you first need a model. That's the second goal of this checkpoint.

-   `Evapotranspiration (ETo) increases with higher air temperature and decreases with higher precipitation.`
-   \*Looked online for statistical notation !\*

$$
\begin{align}
{Eto} &\sim{Gamma(α,λ)}
\end{align}
$$

$$
\begin{align}
ET_0 = β0 + β1(Precipitation) + β2(Temperature)
\end{align}
$$

-   Evapotranspiration (ETo) is driven by vapor pressure deficit, radiation, and temperature. On days with higher precipitation, ETo tends to decrease because of cloud cover, lower radiation, and higher humidity.

2)  Describe your model in statistical notation using the appropriate response family, link function, and predictors. Then use your model to state a statistical hypothesis. Using the wildfire lab again as an example, your statistical hypothesis would be "H0: β_1 = 0; HA: β_1 \> 0".

-   I model daily ETo for the Camarillo station using:

$$
\begin{align}
Precipitation: 
H0 : B1 = 0 \\
HA : B1 < 0 \\
\end{align}
$$

*(Eto decreases on wetter days)*

$$
\begin{align}
Temperature: 
H0 : B1 = 0 \\
HA : B1 > 0
\end{align}
$$

*(Eto increases with temperature)*

-   Eto = evapotranspiration (inches)
-   Precipitation = Daily Precipitation (inches)
-   Temperature = Average Daily Air Temperature (F Degrees)
-   Using a Gamma Model and a link of a log allows to have fitted values of 0-1 remain positive.

## References
- CIMIS. Cimis.water.ca.gov. https://cimis.water.ca.gov/WSNReportCriteria.aspx
