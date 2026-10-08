# Python Project – Electric Vehicle Data Analysis

By Akhil Binjola

Exploratory + inferential analysis of EV specs in Poland (price in PLN, WLTP range, battery, power).

## Files
- `PyhtonProject .ipynb` – all analysis (Tasks 1–5)
- `FEV-data-Excel.xlsx` – source dataset (Make, Model, price, range, battery, energy consumption, engine power)

Video: https://drive.google.com/file/d/1aqT37j75az0mr4tbvoOunNLCtzyA1RN6/view?usp=sharing

## Tasks
1. **Budget + range filter** – EVs ≤ 350,000 PLN and ≥ 400 km range; avg battery by Make. Finding: Tesla/VW/Kia/Hyundai best value vs Audi/Mercedes.
2. **Outlier check** – IQR on `mean - Energy consumption [kWh/100 km]` (bounds ~4.59–33.94). Result: no outliers.
3. **Battery vs Range** – scatterplot + Pearson r ≈ 0.81, strong positive; some 75–95 kWh models show diminishing returns.
4. **Recommendation function** – `recommend_evs(df)`: input budget/min range/min battery, returns top-3 sorted by range then price.
5. **Hypothesis test** – Welch t-test Tesla vs Audi `Engine power [KM]`, with boxplot.

Tools: pandas, matplotlib, seaborn, scipy.stats

## How to run
1. `pip install pandas matplotlib seaborn scipy openpyxl`
2. Open notebook in Jupyter/Colab, upload `FEV-data-Excel.xlsx`, run all cells.
