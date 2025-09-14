# In-Demand Developer Skills Analysis (2024)

### Project Overview
This project is an end-to-end data analysis initiative focused on identifying current and future trends in the technology landscape. Using the latest **Stack Overflow Developer Survey**, this project demonstrates a complete data analysis lifecycle: from raw data acquisition and cleaning to in-depth analysis and the creation of a professional, interactive dashboard. The final product provides actionable insights for strategic decision-making in the IT consulting space.

---

### Features
* **Multi-Source Data Acquisition:** Programmatically collects data from APIs and performs web scraping to build a robust dataset.
* **Comprehensive Data Wrangling:** Cleans, handles duplicates, and imputes missing values to ensure data integrity.
* **Statistical & Exploratory Analysis:** Uncovers data distributions and trends using Python, providing a foundation for formal reporting.
* **Dual-Platform Visualization:** Creates initial exploratory plots with Python and final, interactive dashboards with a Business Intelligence tool.
* **Strategic Insights:** Generates a professional report that informs talent acquisition and skill development strategies.

---

### Technologies Used
* **Programming Language:** Python
* **Data Analysis & Manipulation:** **Pandas**, NumPy
* **Web & API Interaction:** `requests`, **BeautifulSoup**
* **File Handling:** `openpyxl`
* **Data Visualization:** Matplotlib, Seaborn, and **IBM Cognos Analytics**

---

### Project Workflow: A Detailed Breakdown

#### 1. Data Sourcing
The project began by acquiring data from multiple channels to ensure a comprehensive and well-rounded analysis.
* **API Integration:** Used the **`requests`** library to connect to a jobs API, writing Python functions to query and count job postings by technology and location. This data was then exported to an Excel file using **`openpyxl`** for further analysis.
* **Web Scraping:** Deployed **`BeautifulSoup`** to extract structured data from a static HTML web page. The script was designed to navigate the page's HTML to locate and parse key data points, such as programming language names and average annual salaries.
* **Survey Dataset:** The core of the analysis was the **Stack Overflow Developer Survey**, a large CSV dataset containing a wide range of information on developer demographics and technology preferences.

#### 2. Data Wrangling & Cleaning
Once the data was collected, a rigorous cleaning process was performed to ensure its quality and reliability.
* **Duplicate Handling:** Identified and removed 154 duplicate rows from the main dataset, ensuring each response was unique.
* **Missing Value Imputation:** Strategically handled null values in key columns. For categorical data, such as `WorkLoc`, missing entries were filled with the most frequent value. For numerical data like `Age`, the median was used to avoid skewing the distribution.
* **Data Normalization:** A new column, `NormalizedAnnualCompensation`, was created. This was a critical step that converted all salaries (paid yearly, monthly, or weekly) into a single, standardized annual figure, enabling accurate and direct comparison across all respondents.

#### 3. Exploratory Data Analysis & Visualization
With the data cleaned, the project moved into the analysis and visualization phase.
* **Python Visualizations:** Utilized Python libraries **Matplotlib** and **Seaborn** to perform a detailed exploratory data analysis (EDA). Histograms were used to visualize the distribution of key variables, and box plots helped in identifying outliers, ensuring the integrity of subsequent analysis.
* **Cognos Dashboards:** The cleaned and analyzed data was then used to create a series of interactive dashboards in **IBM Cognos Analytics**. These dashboards serve as the final deliverable, providing a clear and professional overview of the project's key findings.
    * **Current Usage Dashboard:** Shows the most popular technologies today.
    * **Future Trends Dashboard:** Highlights technologies that developers want to learn next year.
    * **Demographics Dashboard:** Breaks down the respondent pool by age, gender, country, and education level.

---

### Key Insights
The dashboards revealed several critical insights for any organization staying competitive in the tech sector:
* **Python, JavaScript, and Java** remain the most in-demand programming languages, forming the cornerstone of most job requirements.
* **PostgreSQL** and **MySQL** continue to dominate the database landscape, while NoSQL technologies like **MongoDB** show strong growth.
* There's a significant and growing interest in languages like **Rust** and **Go**, indicating an emerging trend that will influence future hiring needs.

---

### Repository Structure
