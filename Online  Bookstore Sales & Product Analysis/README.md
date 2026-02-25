# Online Bookstore Sales & Product Analysis

This file contains a full project workflow for analyzing an online bookstore's book sales, pricing trends, customer ratings and stock availability. This project includes web scraping, Python analysis, Business Requirements Document (BRD), Business Report and presentation file.

---

##  Project Overview

The goal of this project is to help the online bookstore make **data-driven decisions** regarding:

- Pricing strategy  
- Inventory management  
- Marketing and promotional campaigns  

Currently, the management lacks clear visibility into which books are popular, overpriced or out of stock. This project addresses that gap using real data analysis and business insights.

---
## Dataset : books_dataset.csv

---

## Tools & Technologies Used

- **Python**: pandas, numpy, requests, BeautifulSoup, matplotlib, seaborn, plotly  
- **Jupyter Notebook**: For development and exploration  
- **MS Word / PDF**: BRD and business report  
- **PowerPoint / Google Slides**: Presentation  

---

##  Workflow

### 1. Web Scraping
- Collect book data from online bookstore websites.
- Extract the following fields:
  - `product_id`, `product_name`, `price`, `rating`, `availability`, `product_url`.
- Save cleaned data into `books_dataset.csv`.

### 2. Data Cleaning & Preprocessing
- Handle missing or inconsistent values.
- Convert ratings to numerical format.
- Normalize price and stock data for analysis.

### 3. Data Analysis & KPIs
- Compute key metrics:
  - Average Book Price  
  - Stock Availability Ratio  
  - Rating Distribution  
  - Top 10 Expensive Books  
  - Top 10 Highly Rated Books  
- Answer business questions like:
  - Which books are most expensive / cheapest?  
  - Which books have the highest or lowest ratings?  
  - Which books are trending or underperforming?  

### 4. Business Report & Insights
- Transform data insights into **business-focused recommendations**:
  - Pricing adjustments
  - Inventory management strategies
  - Marketing campaigns

### 5. Presentation
- Summary of findings and recommendations.
- Visualizations for stakeholders.
- Highlight KPIs, insights, and action points.

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/tama81185/All-Profile-Project.git
cd "Online  Bookstore Sales & Product Analysis"
