# Evapo-transpiration and Temperature in Camarillo, California

## Using California Irrigation Management Information System (CIMIS)- Eddy Covariance Station

Final Project - EDS 222 Statistic For Environmental Data Science

# Statistical Notation:

$$ 
\begin{align}
    {Eto} &\sim{Gamma(\mu,\phi)}
\end{align}
$$

$$
\begin{align}
log(\mu) = β0 + β1(Precipitation) + β2(Temperature)
\end{align} 
$$

# Hypothesis:

$$
\begin{align}
Precipitation: 
H0 : B1 = 0 \\
HA : B1 < 0 \\
\end{align}
$$

$$
\begin{align}
Temperature: 
H0 : B1 = 0 \\
HA : B1 > 0
\end{align}
$$

-   Eto = evapotranspiration (inches)
-   Precipitation = Daily Precipitation (inches)
-   Temperature = Average Daily Air Temperature (F Degrees)
-   Using a Gamma Model and a link of a log allows to have fitted values of 0-1 remain positive.

## References

-   CIMIS. Cimis.water.ca.gov. [CIMIS](https://cimis.water.ca.gov/WSNReportCriteria.aspx)
