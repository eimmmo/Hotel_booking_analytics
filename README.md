# Smart Decisions with Hotel Booking Analytics

This project analyzes real-world inspired hotel booking data from a city and a resort hotel.  
It focuses on cancellation behavior, customer segmentation, and seasonal trends to help hotels make smarter, data-driven decisions.

## 📌 Objectives

- Understand guest booking behavior  
- Identify patterns and risk factors in cancellations  
- Explore seasonal demand and market segment trends  
- Deliver actionable business recommendations

## 📊 Dataset Overview

- **Source:** Hotel Booking Demand Dataset  
- **Period:** July 2015 – August 2017  
- **Records:** 119,390  
- **Hotels:** City Hotel & Resort Hotel  
- **Features:** 32 columns  
- **Key Columns:**  
  `is_canceled`, `lead_time`, `arrival_date`, `deposit_type`, `customer_type`, `adr`, `market_segment`, `total_of_special_requests`

## 🛠️ Data Processing

### Cleaning
- Imputed missing values
- Removed outliers (Z-score and IQR)
- Standardized formats and types
- Dropped invalid rows

### Feature Engineering
- Created new features:  
  `total_guests`, `total_nights`, `is_family`, `season`, `country_cancel_ratio`, etc.
- Correlation analysis to find predictors for cancellation

## 📈 Exploratory Data Analysis (EDA)

Key findings:

- ~37% of bookings were canceled  
- Higher cancellation in city hotels and long lead-time bookings  
- Families preferred resort hotels, especially in summer  
- More special requests = fewer cancellations  
- Guest type and deposit type affect behavior

## 📊 Dashboards

### Tools:
- Streamlit  
- tkinter GUI (with ttkbootstrap)  
- Seaborn / Matplotlib

### Features:
- Filter by hotel, year, customer type, season
- Visualize cancellations, ADR, special requests
- Segment guests and bookings
- Cancellation predictors

## ✅ Recommendations

- Require deposits for long lead-time bookings  
- Promote non-refundable bookings  
- Use customer type and request count for targeting  
- Adjust pricing by season  
- Focus marketing on high-value regions  
- Diversify booking channels (reduce OTA dependency)

## 📁 Folder Structure

```
Hotel_Booking_Analytics/
├── data/
│ ├── hotel_bookings.xlsx
│ └── Updated_data.xlsx
│
├── notebooks/
│ └── IEEE Project.ipynb
│
├── dashboards/
│ ├── DashBoard.py
│ └── GUI DashBoard.py
│
└── README.md
```


## 📄 File Descriptions

| File Path                        | Description                                             |
|----------------------------------|---------------------------------------------------------|
| `data/hotel_bookings.xlsx`       | Raw dataset before any processing                      |
| `data/Updated_data.xlsx`         | Cleaned and preprocessed dataset used for analysis     |
| `notebooks/IEEE Project.ipynb`   | Full notebook: cleaning, EDA, visualizations           |
| `dashboards/DashBoard.py`        | Streamlit dashboard for interactive data exploration   |
| `dashboards/GUI DashBoard.py`    | GUI dashboard built using tkinter and ttkbootstrap     |

## ▶️ How to Run

```bash
# Install required packages
pip install pandas numpy seaborn matplotlib streamlit ttkbootstrap

# Run Streamlit dashboard
streamlit run dashboards/DashBoard.py


📬 Contact
Open an issue or fork the project to contribute.

