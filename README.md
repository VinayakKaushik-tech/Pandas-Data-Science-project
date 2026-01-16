Sales Data Analysis: Electronics Store 📈
Project Overview
This project performs a comprehensive analysis of 12 months of electronics store sales data to uncover actionable business insights. By processing hundreds of thousands of transactions, I identify high-value products, peak sales periods, and geographic trends to help optimize marketing and inventory strategies.

🛠 Tech Stack
Python: The core programming language used.

Pandas: For data cleaning, merging, and complex transformations.

Matplotlib: For creating data visualizations.

Jupyter Notebook: For interactive development and documentation.

📊 Key Business Questions Addressed
What was the best month for sales? How much was earned that month?

What city sold the most product?

What time should we display advertisements to maximize the likelihood of customers buying products?

What products are most often sold together?

What product sold the most? Why do you think it sold the most?

⚙️ Technical Workflow
1. Data Cleaning & Preparation
Before analysis, I performed several preprocessing steps to ensure data integrity:

Merging: Combined 12 individual CSV files into a single master DataFrame using pd.concat.

Handling Missing Values: Identified and dropped NaN rows.

Filtering: Cleaned "dirty" data, specifically rows where column headers were repeated within the dataset.

Type Conversion: Used pd.to_numeric and pd.to_datetime to ensure data types were optimized for mathematical and time-series operations.

2. Feature Engineering
I extracted specific details from the raw data to enable more granular analysis:

Month/Hour Columns: Parsed from "Order Date" to find seasonal and daily trends.

City Column: Extracted city and state from "Purchase Address" using .apply() to avoid duplicate city names (e.g., Portland, ME vs. Portland, OR).

Sales Column: Calculated by multiplying Quantity Ordered and Price Each.

3. Data Visualization
Using Matplotlib, I created various charts (Bar, Line, and Subplots) to visualize the findings, making the data accessible for non-technical stakeholders.

🚀 How to Run
Clone the repo:

Bash

git clone https://github.com/VinayakKaushik-tech/Pandas-Data-Science-project.git
Install dependencies:

Bash

pip install pandas matplotlib jupyter
Run the analysis: Open the .ipynb file in Jupyter Notebook or VS Code and run all cells.

📂 Project Structure
Sales_Analysis.ipynb: The main notebook containing all code and visualizations.

Sales_Data/: Folder containing the 12 original CSV files.

all_data.csv: The final cleaned and merged dataset.
