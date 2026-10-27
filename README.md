# Electric Vehicle Market Analysis and Recommendation

A Python data analysis of an electric vehicle (EV) specifications dataset. It combines exploratory analysis, outlier detection, correlation analysis and hypothesis testing, and ends with a function that recommends cars for a buyer's budget and range needs.

## Questions explored

1. Which EVs fit a budget of 350,000 PLN and offer 400+ km of range?
2. Are there vehicles with unusual energy consumption?
3. How strongly does battery capacity relate to driving range?
4. Is there a significant difference in engine power between Tesla and Audi models?

## Methods and findings

| Step | Method | Result |
|---|---|---|
| Shortlisting | Filtering on price and range | Cars under 350,000 PLN with a range of 400+ km |
| Outliers | IQR method on energy consumption | Vehicles with unusually high or low consumption flagged |
| Correlation | Pearson correlation | Strong positive correlation between battery capacity and range (r = 0.81) |
| Hypothesis test | Welch's t-test, Tesla vs Audi engine power | p = 0.107, so no statistically significant difference at the 5% level |
| Recommendation | Interactive function | Returns the top 3 EVs for a user's budget, range and battery needs |

## Tech stack

Python, Pandas, SciPy, Matplotlib, Seaborn, Jupyter / Google Colab.

## How to run

```bash
git clone https://github.com/AkhilBinjola/Python-Project
cd Python-Project
pip install -r requirements.txt
jupyter notebook
```

The notebook reads the Excel dataset from `/content/` (Google Colab). To run locally, change the file path in the loading cell.

## Author

Akhil Binjola · [LinkedIn](https://linkedin.com/in/akhilbinjola) · [GitHub](https://github.com/AkhilBinjola)
