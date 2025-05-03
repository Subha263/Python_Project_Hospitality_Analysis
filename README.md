🏨 Hospitality Domain Data Analysis Using Python
📌 Project Objective This project analyzes booking, customer behavior, and performance metrics from a hospitality company to uncover insights and identify areas for competitive advantage.

💡 Key Business Questions Addressed
What is the booking trend across room categories?
Which cities have the highest average customer ratings?
What is the occupancy rate trend over time?
Which booking platforms drive the most revenue?
Are there patterns based on weekdays vs. weekends?

🗂️ Dataset Description
The project uses 7 CSV files with fields like:
property_id, check_in_date, room_category, successful_bookings, revenue_realized
customer_id, ratings_given, booking_platform, city, capacity, occ_pct

🛠️ Tools & Libraries
Python (Jupyter Notebook)
pandas, matplotlib, seaborn

🔄 Project Workflow

1️⃣ Data Loading
Imported 7 CSV files into the Jupyter Notebook using pandas.
Previewed each dataset using .head(), .info(), and .shape() to understand structure and completeness.
2️⃣ Data Cleaning & Preparation
✅ Date Parsing:
Converted mixed date formats (1/5/2022, 1-5-2022) to datetime using pd.to_datetime() with custom logic.
✅ Handling Missing Values:
Filled missing values in capacity, occ_pct, and other key columns using median or appropriate imputation.
✅ Removing Duplicates:
Checked for and removed duplicate rows in all datasets.
✅ Outlier Detection:
Identified outliers using IQR method in numerical columns like revenue_realized, ratings_given.
✅ Data Type Conversion:
Ensured consistent formats for analysis: int, float, datetime, category.
3️⃣ Exploratory Data Analysis (EDA)
Performed several insights and business-focused analyses:
📌 Booking Behavior
Trend of successful bookings by room category.
Distribution of bookings by city and platform.
📌 Revenue Insights
Total revenue realized by each booking platform (Pie Chart).
Top revenue-generating cities.
📌 Occupancy Insights
Occupancy percentage across weekdays vs weekends (using merged date dimension).
Analysis of properties with highest capacity and booking success.
📌 Ratings Analysis
Average ratings given by city (Horizontal Bar Chart).
Relationship between room class and customer feedback.
4️⃣ Visualization
Used matplotlib and seaborn to create:
Line plots, bar charts, and pie charts for all key KPIs.
Visual storytelling to support insights (custom titles, labels, axis control).
