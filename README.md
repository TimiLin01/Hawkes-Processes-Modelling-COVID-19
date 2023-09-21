# Hawkes-Processes-Modelling-COVID-19
This is the Code Appendix to my Master thesis: Hawkes Processes Modelling of the COVID-19 Pandemic in Israel Using Whittle Estimation Method.

## The data set
The main data set used in this project is too large and, therefore, cannot be uploaded.
It can be downloaded from the [Israeli government website](https://data.gov.il/dataset/covid-19/resource/d07c0771-01a8-43b2-96cc-c6154e7fa9bd) or can be found from [my Google docs](https://drive.google.com/file/d/1VCAGfQwqVdHMn2CCShr195c4kTr94bS8/view?usp=sharing).

Description for other data sets:
- **geo_population.xlsx**: Population data for each town summarised from [Central Bureau of Statistics website](https://www.cbs.gov.il/en/settlements/Pages/default.aspx?mode=Yeshuv).
- **geo_area_loc_std.csv**: Includes the daily cases, seven-day average cases, standardised daily cases and standardised seven-day average cases by dates, areas and towns. Created from the `geo_area_loc.csv` with Excel and `geo_population.xlsx`.
  - daily cases and seven-day average cases are from `geo_area_loc.csv`. Check the `Dissertation_Codes.Rmd` in the *codes* file to see how `geo_area_loc.csv` is produced.
  - By dividing the daily cases and seven-day average cases using the population data in `geo_population.xlsx`, we get the standardised daily cases and standardised seven-day average cases for each town.

## The Code
The `Dissertation_Codes.Rmd` in the *codes* file contains the main codes for the project. Including data cleaning, manipulation, plotting figures, fitting models, etc.
There is also one important source code used, which is the `whittle_periodogram.R` from [Cheysson's GitHub page](https://github.com/fcheysson/code-spectral-hawkes/tree/master/case%20study).
