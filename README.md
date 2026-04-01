# Airbnb Listings EDA Project: New York 2024

---

## :movie_camera: Project Overview

Ever wondered why some Airbnb listings cost 10x more than others in the same city? This project dives deep into **20,765 real Airbnb listings** from New York City (2024) to uncover the factors that drive pricing, availability, and guest satisfaction.

Using **Pandas, NumPy, Matplotlib, and Seaborn**, the analysis covers data cleaning, feature engineering, univariate & bivariate analysis, outlier detection, and actionable recommendations for both guests and hosts.

---

## :bar_chart: Executive Dashboard


  Airbnb Dashboard



---

## :open_file_folder: Dataset at a Glance

| :pushpin: Detail | :chart_with_upwards_trend: Value |
|---|---|
| **Total Listings** | 20,765 |
| **Boroughs Covered** | 5 (Manhattan, Brooklyn, Queens, Bronx, Staten Island) |
| **Features** | 22 columns |
| **Avg Nightly Price** | $187.71 |
| **Price Range** | $10 -- $100,000 |
| **Median Price** | $125 |
| **Most Expensive Borough** | Manhattan ($204/night) |
| **Most Common Room Type** | Entire home/apt |

### :page_facing_up: Key Columns

| :label: Category | :pencil: Fields |
|---|---|
| Listing Info | ID, Name, Neighbourhood, Borough, Latitude, Longitude |
| Host Info | Host ID, Host Name, Calculated Host Listings Count |
| Room Details | Room Type, Bedrooms, Beds, Baths |
| Pricing | Price, Price per Bed (engineered) |
| Reviews | Number of Reviews, Reviews per Month, Last Review, Rating |
| Availability | Availability (365 days), Minimum Nights |

---

## :fire: Key Findings

:small_orange_diamond: **Manhattan** is the most expensive borough at **$204/night** avg, followed by Brooklyn ($155) and Queens ($122)

:small_orange_diamond: **Entire home/apt** is the most common room type (~53%), followed by Private rooms (~41%)

:small_orange_diamond: **Price per bed** reveals the true cost -- Manhattan at **$139/bed** vs Staten Island at just **$68/bed**

:small_orange_diamond: Majority of listings are priced between **$50 - $300**, with extreme outliers up to $100,000

:small_orange_diamond: Listings with **higher availability** tend to have **lower prices and more reviews** -- indicating better guest experiences

:small_orange_diamond: Some hosts manage **multiple listings**, suggesting a growing trend toward **professional hosting**

:small_orange_diamond: **Weak correlation** between price and number of reviews -- expensive doesn't always mean popular

---

## :gear: Analysis Workflow

```
Step 1: Import Dependencies (Pandas, NumPy, Matplotlib, Seaborn)
         |
Step 2: Load Dataset (20,765 listings, 22 features)
         |
Step 3: Initial Exploration (shape, info, describe, nulls)
         |
Step 4: Data Cleaning (handle nulls, fix dtypes, remove outliers)
         |
Step 5: Univariate Analysis (price distribution, room types, boroughs)
         |
Step 6: Feature Engineering (Price per Bed)
         |
Step 7: Bivariate Analysis (price vs borough, reviews vs price, geo plots)
         |
Step 8: Correlation Analysis (heatmap, pairplot)
         |
Step 9: Insights & Recommendations
```

---

## :art: Visualizations Created

| :chart_with_upwards_trend: Chart | :bulb: Insight |
|---|---|
| **Bar Plot** -- Price by Borough x Room Type | Manhattan entire homes are the priciest segment |
| **Scatter Plot** -- Reviews vs Price by Borough | High-priced listings don't always get more reviews |
| **Pair Plot** -- Price, Nights, Reviews, Availability | Availability and reviews show inverse relationship with price |
| **Heatmap** -- Correlation Matrix | Beds and price have moderate positive correlation |
| **Geo Scatter** -- Lat/Long by Room Type | Manhattan is densely packed with entire home listings |
| **Histogram** -- Price Distribution | Right-skewed; most listings under $300 |
| **Box Plot** -- Host Listings Count | Identifies professional hosts with 10+ listings |

---

## :hammer_and_wrench: Tech Stack

| Layer | Tool |
|---|---|
| Language | Python 3.8+ |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |
| Dataset | Inside Airbnb (New York 2024) |

---

## :file_folder: Project Structure

| File | Description |
|---|---|
| `Jupyter_notebook.ipynb` | Complete EDA notebook with all analysis and visualizations |
| `Airbnb_NewYork_dashboard.png` | Executive dashboard summarizing key metrics |
| `README.md` | Project documentation |

---

## :rocket: How to Run

1. **Clone the repository**
```bash
git clone https://github.com/Nikita-Dongre/Python_Airbnb_Project.git
```

2. **Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn
```

3. **Launch the notebook**
```bash
jupyter notebook Jupyter_notebook.ipynb
```

---

## :chart_with_upwards_trend: Average Price by Borough

| Borough | Avg Price/Night | Avg Price/Bed |
|---|---|---|
| Manhattan | $204 | $139 |
| Brooklyn | $155 | $100 |
| Queens | $122 | $76 |
| Staten Island | $119 | $68 |
| Bronx | $108 | $75 |

---

## :bulb: Recommendations

### For Guests :suitcase:
- **Budget travelers**: Look for private rooms in Queens or Bronx -- best value under $80/night
- **Families**: Brooklyn offers spacious entire homes at lower rates than Manhattan
- **Check reviews**: Listings with high availability + many reviews = consistent quality
- **Avoid outliers**: Filter out listings above $1,000 to find realistic options

### For Hosts :house_with_garden:
- **Price competitively** based on borough and room type benchmarks above
- **Maximize availability** -- higher availability correlates with more bookings and reviews
- **Encourage reviews** -- they directly improve listing visibility
- **Multi-listing strategy**: Consider managing multiple properties for higher total revenue

---

## :crystal_ball: Future Work

- :robot: **Machine Learning** -- Predict prices using room type, location, and amenities
- :speech_balloon: **Sentiment Analysis** -- Analyze review text to understand guest satisfaction drivers
- :world_map: **Interactive Dashboard** -- Build a Plotly/Tableau dashboard for live exploration
- :calendar: **Time Series** -- Track seasonal pricing trends across months

---

## :dart: Conclusion

This project reveals that **location and room type are the strongest price drivers** in the NYC Airbnb market. Manhattan dominates in pricing, but Brooklyn offers the best balance of quality and affordability. The analysis provides actionable insights for both guests seeking value and hosts optimizing revenue -- all through the power of Python EDA.

---

## :handshake: Author


  Nikita Dongre

  Data Enthusiast | Python Analytics | Aspiring Data Analyst




  :star: If you found this project insightful, give it a star!



---


  Made with :heart: and Python

