# London Bike Sharing — Exploratory Data Analysis

## About the project

This is a personal Data Science project where I explored how bike rental demand in London changes depending on the time of day, temperature and weather conditions. I used Python to analyse the data, create visualisations and compare different groups of observations.

The dataset contains **17,414 hourly records** from January 2015 to January 2017.

## Questions I explored

- When are bike rentals most common during the day?
- How do rental patterns differ between weekdays and weekends?
- How is temperature related to bike rental demand?
- Are there differences between rainy and non-rainy hours, including at similar temperatures or times of day?

## Tools and methods

- **Python** and **Pandas** for loading, preparing and analysing data
- **Matplotlib** (through Pandas plotting) for charts
- Descriptive statistics, grouping and comparisons of hourly averages
- Converting timestamps, checking for missing values and creating new variables

## Main findings

- Bike rentals peak around **8 AM** and **5 PM**, which may be related to commuting.
- Weekday demand has clear morning and evening peaks, while weekend demand is more spread out across the afternoon.
- Average rentals generally increase with temperature. The highest average is in the **25–30°C** group, although very hot temperature groups have fewer observations.
- Rainy hours have lower average rentals than non-rainy hours across the temperature groups where both conditions are observed.
- The morning and evening peaks are still visible in rainy conditions, but at lower levels.

These results show associations in this dataset, not proof that weather or commuting causes the differences.

## Limitations

Some weather and temperature groups have relatively few observations. I also compared factors such as temperature and time of day separately rather than controlling for all variables at once. Other factors may help explain the patterns.

## Dataset

[London Bike Sharing Dataset on Kaggle](https://www.kaggle.com/datasets/hmavrodiev/london-bike-sharing-dataset), based on Transport for London open data.

For this analysis, I classified weather codes **7** and **10** as rainy. This uses weather categories rather than measured rainfall amounts.

## How to view or run the analysis

Open the `.ipynb` file in Jupyter Notebook or Kaggle to view the code, explanations and charts.

The notebook was created on Kaggle and reads the CSV from a Kaggle input path. To rerun it on Kaggle, attach the linked dataset as an input and select **Run All**. To run it locally, download `london_merged.csv` from the dataset page and change the path in `pd.read_csv()` to its location on your computer.

## What I learned

This project gave me more practice with Pandas, data visualisation and interpreting results carefully. It also helped me understand why sample size and other variables matter when comparing groups.
