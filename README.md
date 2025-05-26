📊 Paper Machine Efficiency Calculator
This project simulates the efficiency monitoring of a paper manufacturing machine using Python. It calculates Overall Equipment Effectiveness (OEE) and provides insights into production performance and downtime causes.

✅ Features
Calculates OEE components: Availability, Performance, and Quality

Analyzes and summarizes downtime reasons

Generates a recommendation report for improving machine efficiency

Works with CSV or built-in sample datasets

Fully written in Python and compatible with Google Colab

🧠 Learning Objectives
Practice defining and using functions

Understand parameters and return values

Use DataFrames and basic statistics in Python

Apply functional programming and code documentation with docstrings

📁 Dataset
The project uses a dataset containing the following columns:

runtime

downtime

planned_production_time

total_produced

waste

ideal_output

downtime_reason

You can either:

Upload your own CSV file in Google Colab

Use the built-in sample dataset provided in the code

🚀 How to Run (Google Colab)
Open Google Colab

Copy and paste the full code into a new notebook

(Optional) Upload your .csv file:

python
Copy
Edit
from google.colab import files
uploaded = files.upload()
Load your CSV:

python
Copy
Edit
import pandas as pd
df = pd.read_csv("your_file_name.csv")
Generate the report:

python
Copy
Edit
generate_report(df)
🛠️ Example Code Snippet
python
Copy
Edit
metrics = calculate_oee(df)
generate_report(df)
📈 Sample Output
yaml
Copy
Edit
===== MACHINE EFFICIENCY REPORT =====
Availability : 88.89%
Performance  : 95.45%
Quality      : 95.83%
OEE          : 81.03%

--- Downtime Reasons ---
Maintenance: 2
Breakdown: 1

--- Recommendations ---
- Reduce downtime to improve availability.
📚 References
Overall Equipment Effectiveness

Python Functions Guide

TAPPI - Paper Machine Efficiency Metrics

💡 Future Improvements
Add chart visualizations using matplotlib or seaborn

Export the report as a .txt or .pdf

Create a web dashboard version using Streamlit









