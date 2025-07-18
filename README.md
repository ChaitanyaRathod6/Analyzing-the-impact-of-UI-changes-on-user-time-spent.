📊 Analyzing the Impact of UI Changes on User Engagement

This project analyzes whether a new user interface (UI) design improves user engagement, specifically focusing on time spent, page clicks, and scroll depth. The project mimics a typical A/B testing scenario used by top tech companies like Meta, Netflix, and Google.

📁 Project Structure
bash
Copy
Edit

.
├── ui_engagement_dataset_final.csv        # Cleaned dataset with full datetime

├── analysis.ipynb                         # Jupyter notebook with full analysis

├── README.md                              # Project documentation

🧠 Objective

Determine whether a newly deployed UI leads to better user engagement by analyzing key metrics and validating results statistically.

🧾 Dataset Description
Column	Description
user_id	Unique ID of the user
session_id	Unique ID of the session
ui_version	UI version used (Old or New)
time_spent_seconds	Total time spent in the session (sec)
page_clicks	Number of pages clicked in session
scroll_depth	Scroll depth during session (0 to 1)
datetime	Timestamp of session start
date_formatted	Formatted date in DD-MM-YYYY format

🔍 Project Steps
✅ 1. Data Cleaning & Preparation
Checked for missing values and duplicates

Added formatted date column (DD-MM-YYYY)

Ensured data types were consistent

📊 2. Exploratory Data Analysis (EDA)
Compared metrics across ui_version

Visualized average time spent, clicks, and scroll depth

🧪 3. Statistical Testing
Performed independent T-tests to assess:

Time spent

Page clicks

Scroll depth

Found significant improvement with new UI

🤖 4. Predictive Modeling (Optional)
Built a linear regression model to predict time_spent_seconds

Key features: ui_version, page_clicks, scroll_depth

Evaluated performance using RMSE

📌 Key Findings
Users spent more time with the new UI

Page clicks and scroll depth were higher in the new UI

All differences were statistically significant (p < 0.05)

💡 Recommendations
Fully roll out the new UI

Continue A/B testing on individual UI components

Track post-rollout metrics to ensure sustained success

Segment analysis by user type (e.g., mobile, new users)

🛠️ Tech Stack
Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn, SciPy, scikit-learn

📎 How to Run
Clone or download the repository.

Open the analysis.ipynb file in Jupyter or Google Colab.

Run each cell in order to replicate the full analysis.
