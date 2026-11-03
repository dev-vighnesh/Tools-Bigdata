# Bike Sharing Demand: Statistical Analysis & Operational Insights 🚲📊

## Overview
This project analyzes the environmental and temporal factors that drive bike-sharing demand. Using the **UCI Bike Sharing dataset** (over 17,000 hourly observations), this notebook explores how commuter schedules, working days, and seasonal weather patterns affect rider behavior. 

Beyond exploratory data analysis, the project heavily relies on **statistical inference** to bridge the gap between mathematical significance and practical, operational business decisions.

## Key Insights
* **Commuter vs. Leisure Patterns:** Demand is heavily dictated by working day schedules, displaying massive commuter spikes at 8:00 AM and 5:00 PM. Weekends show a smooth, gradual bell curve peaking in the early afternoon.
* **The Seasonal Shift:** Statistical testing (Z-test for two proportions) confirmed a massive operational shift between seasons. During the warmest season (Fall), nearly 19% of hours qualify as "high-demand" (>400 rentals), compared to just 3.8% in the coldest season (Spring).
* **Business Recommendations:** Bike fleet operations must implement dynamic daily reallocation (moving bikes to residential hubs before 8 AM and commercial hubs before 5 PM) and aggressively scale down the active fleet during colder seasons to optimize maintenance resources.

## Tech Stack
* **Python 3**
* **Pandas & NumPy:** Data manipulation and transformation
* **Matplotlib & Seaborn:** Exploratory data visualization
* **SciPy (`scipy.stats`):** Inferential statistics (Welch's t-test, Z-test for proportions, Pearson correlation)

## How to Run Locally
1. Clone this repository to your local machine.
2. Ensure you have the required libraries installed:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy
   ```
3. Verify that `hour.csv` is located in the same directory as the Jupyter Notebook.
4. Launch Jupyter and run the notebook:
   ```bash
   jupyter notebook Bike_Sharing_Demand_Analysis.ipynb
   ```

## Repository Structure
* `Bike_Sharing_Demand_Analysis.ipynb`: The main notebook containing all code, visualizations, and analytical write-ups.
* `hour.csv`: The hourly aggregated dataset.

## Data Source
Fanaee-T, Hadi, and Gama, Joao. *Bike Sharing Dataset*. UCI Machine Learning Repository, 2013.