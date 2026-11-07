# econ3916-midterm
# What is an extra 100 square feet worth? Living area and house prices in Ames, Iowa

ECON 3916 Midterm Project, Fall 2026

## Question

In home sales in Ames, Iowa between 2006 and 2010, how much higher is the sale price of a home with 100 more square feet of above-ground living area, holding neighborhood, overall quality, year built and year of sale fixed?

## Data

- **Source:** Ames Housing data, assembled by Dean De Cock from records of the Ames City Assessor's Office (De Cock, D. (2011). Ames, Iowa: Alternative to the Boston Housing Data as an End of Semester Regression Project. *Journal of Statistics Education*, 19(3)). This version is the Kaggle "House Prices: Advanced Regression Techniques" training set.
- **Downloaded from:** OpenML, dataset 42165, https://www.openml.org/d/42165, on 2026-11-05.
- **Size:** 1,460 home sales, 81 variables. One row is one residential sale.
- **Copy in this repository:** `data/ames_house_prices.csv`, the data exactly as downloaded.

## How to run

1. Open `midterm_starter.ipynb` and click **Open in Colab** at the top.
2. In Colab, choose **Runtime › Run all**. The notebook downloads the data from OpenML, so it needs an internet connection; all packages it uses are preinstalled in Colab.
3. If OpenML is unavailable, upload `data/ames_house_prices.csv` to the Colab session and replace the `fetch_openml` line with `df = pd.read_csv("ames_house_prices.csv")`.

The notebook produces every number, table and figure in the report. The last code cell prints every number the report quotes.

## Headline finding

Holding neighborhood, quality, age and year of sale fixed, a home with 100 more square feet of living area sold for about **2.75% more** (robust 95% CI 2.16% to 3.35%), roughly US$4,490 for a median-priced home. This is a conditional association, not a causal effect: the model omits features such as lot and basement size that come with larger homes. The estimate rises to 3.18% when the four homes above 4,000 sq ft, including two sales of unfinished homes, are excluded.

## Files

- `midterm_starter.ipynb`: the full analysis
- `report.pdf`: the written report
- `data/ames_house_prices.csv`: the raw data

## Use of AI

I didn't use AI in the project.
