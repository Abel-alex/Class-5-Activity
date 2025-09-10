---
title: "README.md"
author: "Abel Regassa"
date: "2025-09-10"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

Setup
•	Suppresses unnecessary warnings and messages for a cleaner report.
•	Loads the tidyverse package, which bundles together essential tools (dplyr, ggplot2, readr, etc.) for data cleaning, manipulation, and visualization.
________________________________________
Load Data
•	Reads in the raw Class 1 survey dataset directly from GitHub.
•	Uses dim() to quickly check the shape of the dataset (number of rows and columns).
•	This ensures the data was loaded correctly before further steps.
________________________________________
Rename Columns
•	Applies meaningful, standardized names to all 27 variables.
•	Renaming improves readability and makes later analysis easier.
•	Uses glimpse() to preview selected key variables (bday, bmonth, fav_num, like_cats, like_dogs, etc.) so you can confirm they imported correctly.
________________________________________
Clean and Summarize bday and bmonth
•	Keeps the raw versions of bday and bmonth while creating cleaned numeric versions.
•	Converts values into numbers for consistent analysis.
•	Generates frequency tables before cleaning to show the raw distributions.
•	Cleans data by restricting values to plausible ranges (bday: 1–31, bmonth: 1–12).
•	Replaces implausible entries (like 0 or 35) with NA.
•	Creates frequency tables after cleaning to confirm corrections.
________________________________________
Descriptive Statistics
•	Summarizes numeric preferences, especially fav_num (favorite number).
•	Produces count, mean, standard deviation, minimum, median, and maximum values.
•	Helps describe central tendency and variability in the dataset.
________________________________________
Visualizations
•	Histogram of favorite number: shows the distribution and how responses are spread.
•	Bar chart of favorite season: highlights which seasons are most and least preferred.
•	Visuals complement tables by making trends and outliers easier to detect.
________________________________________
Save Cleaned Data
•	Exports the cleaned dataset as class1_survey_clean.csv.
•	This ensures reproducibility—others can work with a standardized, ready-to-analyze dataset.
________________________________________
Session Info
•	Records the R version, platform details, and loaded package versions.
•	Critical for reproducibility, so future users can replicate the analysis in the same environment.

