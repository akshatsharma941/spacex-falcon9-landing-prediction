# SpaceX Launch Data Dashboard

This project is an interactive dashboard built using Plotly Dash to analyze SpaceX launch performance. It allows users to explore how launch site, payload mass, and booster version influence mission success.

---

## Project Overview

The goal of this project is to provide a simple way to explore patterns in SpaceX launch outcomes. The dashboard enables dynamic filtering and visual analysis of launch data, helping identify trends in reliability and performance across different conditions.

---

## Key Features

* Interactive filtering by launch site and payload range
* Visualization of success rates across launch sites
* Comparison of successful vs failed launches for individual sites
* Scatter analysis of payload mass vs mission outcome
* Color-coded booster version performance

---

## Insights

Using the dashboard, users can observe patterns such as:

* Certain launch sites consistently achieving higher success rates
* Variations in success probability across payload ranges
* Differences in performance between booster versions

---

## Tech Stack

* Python
* Pandas
* Plotly Express
* Dash

---

## How to Run

```
pip install pandas dash plotly
python spacex_dash_app.py
```

Then open:

```
http://127.0.0.1:8050/
```

---

## Future Improvements

* Add time-based analysis of launches
* Introduce summary metrics (success rate, total launches)
* Improve layout and styling
* Deploy the application for public access

---

## Notes

This project focuses on interactive data visualization and exploratory analysis. It can be extended further with deeper statistical analysis or additional datasets.

---

Author: Akshat Sharma, 2nd-year CSE Undergrad