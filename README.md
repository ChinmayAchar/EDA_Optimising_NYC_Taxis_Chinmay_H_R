🚖 Optimising NYC Taxi Operations (EDA)
Author: Chinmay H R Project Type: Exploratory Data Analysis / Urban Mobility Tech Stack: Python (Pandas, Seaborn, Matplotlib, Folium)

(Above: Real-time traffic flow visualization concept - representing the dynamic nature of the dataset)

📌 Project Overview
New York City is a complex ecosystem of transit. For taxi operators, efficiency is the difference between profit and loss. This project utilizes Exploratory Data Analysis (EDA) on millions of NYC taxi trip records to uncover hidden patterns in traffic, passenger demand, and trip duration.

Goal: To provide data-driven recommendations that help fleet operators reduce idle time and maximize fare revenue per hour.

📂 Repository Structure
EDA_Assg_NYC_Taxi_Starter_Chinmay_H_R.ipynb: The core analysis notebook containing data cleaning, feature engineering, and visualization code.

Report_NYC_Taxi_Operations_Starter_by_Chinmay_HR.pdf: Executive summary and strategic insights.

README.md: Project documentation.

⚙️ Data Pipeline
The project follows a rigorous data science workflow:

Shutterstock

Data Cleaning:

Removed "Ghost Trips" (negative duration/distance).

Fixed coordinate anomalies (trips starting in the ocean).

Imputed missing values for store_and_fwd_flag.

Feature Engineering:

Speed Calculation: Derived avg_speed_mph to detect congestion.

Time Binning: Segmented day into "Morning Rush", "Mid-day", "Evening Rush", and "Late Night".

Trip Duration: Calculated exact travel times from pickup/dropoff timestamps.

📊 Key Visualizations & Analysis
1. Demand Hotspots (Heatmap Animation)
Understanding where and when demand peaks is crucial. The analysis breaks down demand by hour and day.

(Visualization of demand density shifting throughout the day)

Insight: Demand is highest on Friday Evenings (6 PM - 9 PM) and lowest on Monday Mornings.

Strategy: Drivers should position themselves in Midtown Manhattan during the evening rush to maximize pickup probability.

2. Trip Duration vs. Time of Day
We analyzed how long it takes to travel during different windows.

Observation: Average speed drops to <10 mph during the 5:00 PM - 7:00 PM window.

Impact: While demand is high, the "Time Cost" of traffic reduces profitability per hour.

3. Correlation Matrix
We examined the relationships between distance, fare, and duration.

Key Finding: Trip Duration and Fare Amount are not always perfectly correlated due to "waiting time" charges in heavy traffic.

🚀 Strategic Recommendations
Based on the visual analysis, the following actions are recommended for the client:

Shift Optimization:

Action: Schedule maximum drivers for the Friday-Saturday Night window.

Reason: High demand + faster average speeds (less traffic) = Max Profit.

Route Avoidance:

Action: Avoid cross-town trips in Midtown during Evening Rush (5-7 PM).

Reason: Extremely low speeds reduce the number of possible trips per shift.

Airport Targeting:

Action: Prioritize JFK/LaGuardia trips during Mid-day (11 AM - 3 PM).

Reason: Long-distance fares with moderate traffic offer the best stable revenue.

🛠️ How to Run
Clone the repository.

Install dependencies: pip install pandas matplotlib seaborn folium.

Run the Jupyter Notebook: jupyter notebook EDA_Assg_NYC_Taxi_Starter_Chinmay_H_R.ipynb.
