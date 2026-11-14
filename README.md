# Data Jobs Dashboard | Power BI


## Introduction

This interactive Power BI dashboard was initially developed as part of [Luke Barousse's Power BI for Data Analytics course](https://www.lukebarousse.com/powerbi). It analyzes 2024 data science job postings to help job seekers and career changers explore hiring trends, salary distributions, and employment opportunities.

The report consolidates job market information into two interactive pages, allowing users to compare roles, identify trends, and explore detailed information about specific job titles.

The dataset used in this project was provided through Luke Barousse's course and is available in the [course's GitHub repository](https://github.com/lukebarousse/PowerBI_Data_Analytics_Course/tree/main/Data).

### Dashboard File
You can find the file for the dashboard here: [`Data_Jobs_Dashboard.pbix`](/Data_Jobs_Dashboard.pbix).  

## Skills Showcased

This project demonstrates proficiency in the following Power BI tools and techniques:

-   **Data Transformation (ETL) with Power Query:** Cleaned and prepared raw data by handling missing values, adjusting data types, and creating new columns. Additionally, standardized inconsistent job platform names to ensure accurate grouping and aggregation in visualizations.
-   **Data Aggregation:** Used Power BI's built-in aggregation functions to calculate job metrics such as `Median Yearly Salary` and `Job Count`.
-   **Core Charts:** Utilized **Column, Bar, Line, Scatter, Donut** and **Gauge Charts** to compare job counts and track trends over time.
-   **Geospatial Analysis:** Leveraged **Map Charts** to visualize the global distribution of jobs.
-   **KPI Indicators & Tables:** Used **Cards** to display key metrics and **Tables** to provide granular, sortable data.
-   **Dashboard Design:** Designed an intuitive and visually appealing layout, exploring both common and uncommon chart types to best tell the data story.
-   **Interactive Reporting:**
    -   **Slicers:** To dynamically filter the report by Job Title.
    -   **Buttons & Bookmarks:** To create a seamless navigation experience.
    -   **Drill-Through:** To navigate from a high-level summary to a contextual, detailed view.
---

## Dashboard Overview

*This report is split into two distinct pages to provide both a high-level summary and a detailed analysis.*

### Page 1: High-Level Market View

![Data Jobs Dashboard Page 1](/images/project_1_page_1.png)  

Page 1 provides a high-level overview of the data job market, highlighting key metrics such as total job postings, median salaries, and the most in-demand roles. Interactive visuals allow users to filter results by job title and reporting period, with drill-through functionality providing access to more detailed information about individual roles.

![Filtered Data Jobs Dashboard Page 1](/images/project_1_page_1_filtered.png)  

**Interactive Filtering Example:** Selecting Data Analyst and Q2 2024 updates the dashboard to display approximately 30K matching job postings, along with their corresponding salary metrics and trends.

#### Notes:
The Salary Star Rating evaluates job titles based on their median annual salaries. The rating is calculated using a normalized salary scale ranging from $75,000 to $150,000, with the result rounded to the nearest whole star. Consequently, salaries below $82,500 receive zero stars, while salaries of $142,500 or higher receive five stars. Intermediate ratings are assigned in $15,000 salary increments.


| Star Rating | Median Annual Salary |
|:---:|---|
| ☆☆☆☆☆ (0 Stars) | Below $82,500 |
| ★☆☆☆☆ (1 Star) | $82,500 – $97,499.99 |
| ★★☆☆☆ (2 Stars) | $97,500 – $112,499.99 |
| ★★★☆☆ (3 Stars) | $112,500 – $127,499.99 |
| ★★★★☆ (4 Stars) | $127,500 – $142,499.99 |
| ★★★★★ (5 Stars) | $142,500 and above |



### Page 2: Job Title Drill-Through

![Data Jobs Dashboard Page 2](/images/project_1_page_2.png)  

This is the deep-dive page. From the main dashboard, you can drill through to this view to get specific details for a single job title, including salary ranges, work-from-home stats, top hiring platforms, and a global map of job locations. Users can click the back arrow to go back to the main dashboard and select a different job title.


## Key Findings

-   **Overall Job Market:** The dataset contains approximately 479,000 data-related job postings from 2024, with an overall median reported annual salary of approximately $113,000.
-   **Most In-Demand Roles:** Data Engineer accounted for the largest share of postings (26.9%), followed by Data Analyst (23.6%) and Data Scientist (20.4%).
-   **Remote Work Availability:** Approximately 10% of Data Analyst postings were explicitly identified as offering work-from-home opportunities.

---

## Dataset Limitations
-   **Degree Requirements:** A job posting that does not explicitly mention a degree may still require one.
-   **Health Insurance:** A posting that does not mention health insurance does not necessarily indicate that the employer offers no coverage.
-   **Remote Work:** Job postings not explicitly identified as remote should not automatically be classified as on-site positions.
-   **Salary Data:** Salary statistics are calculated from postings containing available salary information and may not represent all job listings in the dataset.

---

## Conclusion

This project demonstrates how Power BI can be used to transform job posting data into an interactive analytical report. By combining market-level trends with detailed job-title analysis, the dashboard helps users compare career opportunities while showcasing practical skills in data preparation, visualization, and interactive reporting.

