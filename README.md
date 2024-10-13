# InsightsForYOU
You give us the Datasets, and we give you your Insights

A web application built with Flask that allows users to upload datasets (CSV or Excel) and analyze them based on a user-provided prompt. The app extracts key actions and fields from the prompt to perform data analysis like summarizing, comparing, and finding specific data insights.

Features-

Prompt-Based Analysis: Users can enter natural language prompts such as "summarize sales data" or "compare revenue and profit."

File Upload Support: Accepts datasets in CSV and Excel (.xlsx) formats.

Summarize Data: Generates descriptive statistics for the dataset.

Compare Fields: Compares specific columns in the dataset, providing statistical insights.

Find Conditions: Extracts and filters data based on conditions (e.g., "find records between 2020 and 2023").

Graphical Visualizations: Generates basic bar, line, and scatter plots using Matplotlib.


How It Works-

User Uploads Dataset: The user can upload a CSV or Excel file containing the dataset.

Prompt Entry: The user provides a prompt (e.g., "summarize the data" or "compare sales and revenue").

Natural Language Processing (NLP): The app uses spaCy to extract actionable keywords (like compare, summarize, or find) and field names from the prompt.

Data Analysis: Based on the extracted keywords and fields, the application performs the requested action and returns the results.

Visualization: For numerical fields, the app generates basic visualizations to provide graphical insights.


Usage-

Step 1: Upload a CSV or Excel file.

Step 2: Enter a prompt in natural language, such as:
Summarize the data
Compare sales and profit
Find records between 2020 and 2023

Step 3: Click "Analyze" to get the results, which include:
A summary or comparison table
Basic visualizations (bar/line/scatter plots)

Example Prompts-

Summarize Action: Summarize

Compare Action: Compare profit expenses

Find Action: Find data between 2020 and 2022


Supported File Formats

CSV (.csv): Comma-separated value files.

Excel (.xlsx): Excel spreadsheet files.


Technologies Used

Flask: Web framework for Python.

Pandas: For reading and manipulating CSV and Excel data.

spaCy: Natural Language Processing (NLP) library for prompt analysis.

Matplotlib/Seaborn: For basic data visualizations (bar charts, line graphs, scatter plots).

HTML/CSS: Frontend for displaying results.


Folder Structure

.

├── app.py                      # Main Flask application

├── templates

│   └── index.html               # HTML template for the user interface

├── uploads                      # Folder where uploaded files are stored

├── static                       # Static files (CSS, JS, etc.)

├── requirements.txt             # List of required Python packages

└── README.md                    # Project documentation


Future Improvements

Add support for more file types (e.g., JSON).

Introduce interactive visualizations using Plotly.

Generate downloadable PDF reports.

Real-time progress feedback using WebSockets.

Expand NLP capabilities for more complex prompts.


Contributing

Contributions are welcome! If you encounter bugs or have suggestions for improvements, please open an issue or submit a pull request.


License

This project is licensed under the MIT License.
