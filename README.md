# Page View Time Series Visualizer

This project visualizes time series data of daily page views on the freeCodeCamp.org forum using **line plots**, **bar plots**, and **box plots**. It helps identify overall trends, monthly averages, and seasonal patterns.

## 📂 Dataset

The data comes from `'fcc-forum-pageviews.csv'`, containing page views from **2016-05-09 to 2019-12-03**. Each entry represents the total number of page views on a particular day.

---

## ✨ Visualizations

### 📈 Line Plot
- **Function**: `draw_line_plot()`
- **Purpose**: Visualizes daily page views over time.
- **Chart Title**: *Daily freeCodeCamp Forum Page Views 5/2016–12/2019*

### 📊 Bar Plot
- **Function**: `draw_bar_plot()`
- **Purpose**: Shows average monthly page views grouped by year.
- **Legend**: Displays months.
- **Axes**: 
  - X: Years  
  - Y: Average Page Views

### 📦 Box Plots
- **Function**: `draw_box_plot()`
- **Purpose**: Reveals data distribution by:
  - **Year** (trend)
  - **Month** (seasonality)
- Useful for spotting outliers, variance, and recurring monthly patterns.

---

## ⚙️ Data Processing Steps

1. **Import the dataset** and parse the `date` column as a datetime index.
2. **Filter out outliers**: remove the top and bottom 2.5% of values to focus on central trends.
3. **Create three types of plots** using clean data.

---

## 🧪 Sample Usage

```python
from time_series_visualizer import draw_line_plot, draw_bar_plot, draw_box_plot

draw_line_plot()
draw_bar_plot()
draw_box_plot()
📁 Output Files
line_plot.png

bar_plot.png

box_plot.png

🛠️ Requirements
Python 3

pandas

matplotlib

seaborn

bash
Copy
Edit
pip install pandas matplotlib seaborn
🔍 Insights
Are page views increasing over time?

Which months have the highest or lowest activity?

Is there a recurring seasonal pattern in traffic?

This project is excellent practice for:

Time series visualization

Data cleaning and transformation

Advanced plotting with Seaborn and Matplotlib
