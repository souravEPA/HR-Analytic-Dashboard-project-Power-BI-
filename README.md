# HR-Analytic-Dashboard-project-Power-BI-
This project based on the hypothetical data on Nova Peoples HR Solutions. This HR Analytics Dashboard project is very informable and skilled data dependent project made on Power BI. This project highlight my expertise on Power BI software. This helps to increase my skill on power query, DAX formula, Data Visualization, KPI analysis etc.

# 📊 HR Analytics Dashboard | Power BI

**An interactive HR Analytics Dashboard built with Microsoft Power BI to analyze workforce metrics, employee attrition, attendance, salary distribution, hiring trends, and performance.**

This project is a hypothetical HR analytics solution developed for **NovaPeople HR Solutions** to demonstrate business intelligence, data transformation, DAX calculations, KPI development, and interactive data visualization skills.

![Power BI](https://img.shields.io/badge/Power%20BI-Data%20Visualization-F2C811?logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Data%20Modeling-blue)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-green)
![Project Status](https://img.shields.io/badge/Status-Portfolio%20Project-success)

---

## 📌 Project Overview

The **NovaPeople HR Analytics Dashboard** provides a consolidated view of key human resource metrics through an interactive and visually engaging Power BI report.

The dashboard helps HR professionals and management explore workforce composition, employee attrition, salary patterns, attendance status, departmental hiring trends, and performance ratings.

The main objective of this project is to transform HR data into meaningful insights that can support workforce planning, employee retention strategies, and data-driven decision-making.

**Note:** NovaPeople HR Solutions is a hypothetical company created for this portfolio project. All associated data and business scenarios are intended for demonstration purposes and should not be interpreted as actual company information.

## 🎯 Project Objectives

- Analyze overall workforce size and active employee counts.
- Monitor employee attrition and attrition rates.
- Examine hiring trends across departments and quarters.
- Understand employee attendance patterns.
- Compare salary distribution across salary slabs.
- Analyze attrition by department, gender, and reason.
- Evaluate employee performance rating distributions.
- Build an interactive dashboard with department, designation, and location-based filtering.
- Demonstrate practical Power BI, Power Query, and DAX skills.

## 🖥️ Dashboard Preview

![NovaPeople HR Analytics Dashboard](images/hr-analytics-dashboard.png)

*Dashboard preview: workforce KPIs, hiring trends, attendance distribution, attrition analysis, salary distribution, departmental workforce, and performance ratings.*

> **To display your screenshot:** Create an `images` folder in your GitHub repository, upload your dashboard screenshot, and rename it to `hr-analytics-dashboard.png`. Make sure the image path matches the Markdown above.

## 📈 Key Performance Indicators (KPIs)

The dashboard includes the following key metrics, as displayed in the current report.

| KPI | Displayed Value | Purpose |
|---|---:|---|
| Total Employees | 5K | Overview of the workforce |
| Active Employees | 4K | Monitoring the active workforce |
| Average Salary | 57.72K | Understanding average compensation |
| Average Performance | 3.48 | Summarizing employee performance ratings |
| Attrition Count | 569 | Tracking employee departures |
| Attrition Rate | 11% | Monitoring employee attrition |
| Total Attendance | 100K | Summarizing attendance records or events |

*Values are based on the current dashboard screenshot. Units, reporting period, and KPI calculation definitions should be documented alongside the underlying dataset and DAX measures.*

## 📊 Dashboard Features

### 1. Workforce Overview
- Total employee and active employee KPIs.
- Average salary and performance indicators.
- High-level overview of workforce metrics.

### 2. Hiring Trend Analysis
- Hiring trends by department.
- Quarterly comparisons to explore changes in recruitment activity.
- Visual comparison of department-level hiring patterns.

### 3. Attendance Analysis
- Distribution of attendance statuses, including Present, Remote, Leave, Late, and Absent.
- Overview of attendance patterns across the reporting dataset.

### 4. Employee Attrition Analysis
- Attrition by department.
- Attrition according to reason.
- Attrition by gender.
- Attrition count and attrition rate KPIs.

### 5. Salary Analysis
- Attrition by salary slab.
- Comparison of resigned and terminated employee counts across salary categories.
- Exploration of salary distribution and employee exits.

### 6. Performance Analysis
- Distribution of employee performance ratings.
- Comparison of the number of employees across rating levels.

### 7. Departmental Workforce Analysis
- Department-wise employee distribution.
- Comparison of workforce size across departments.

### 8. Interactive Filters
The dashboard includes interactive slicers for:

- **Location:** Barishal, Chattogram, Dhaka, Khulna, Rajshahi, and Sylhet.
- **Designation:** Director, Entry, Junior, Manager, Mid, and Senior.

These slicers allow users to explore workforce metrics for selected locations and designation categories.

## 🛠️ Tools and Technologies

| Tool / Technology | Application |
|---|---|
| Microsoft Power BI Desktop | Dashboard development and report design |
| Power Query | Data cleaning, transformation, and preparation |
| DAX (Data Analysis Expressions) | KPI calculations and analytical measures |
| Data Modeling | Organizing tables and defining relationships, where applicable |
| Interactive Slicers | Filtering and exploring HR metrics |
| Data Visualization | KPI cards, line charts, bar charts, area charts, and donut charts |
| GitHub | Project documentation, version control, and portfolio presentation |

## 🔄 Project Workflow

1. **Data Preparation:** Load the project dataset into Power BI.
2. **Data Cleaning:** Use Power Query to inspect data types, handle missing or inconsistent values, and prepare fields for analysis as required.
3. **Data Modeling:** Organize relevant tables and establish appropriate relationships.
4. **DAX Development:** Create measures for workforce KPIs, attrition analysis, average salary, attendance, and performance.
5. **Visualization:** Build charts and KPI cards to communicate key HR metrics.
6. **Dashboard Design:** Arrange visuals into a consolidated dashboard with a consistent layout and styling.
7. **Interactivity:** Add slicers to support location- and designation-based analysis.
8. **Validation:** Reconcile KPI totals, percentages, filters, and chart values against the underlying data.
9. **Documentation:** Publish the project overview, dashboard screenshot, and relevant project files on GitHub.

## 🧮 DAX Measures

DAX is used to calculate and analyze HR metrics. The following are illustrative examples; adapt the table names, column names, and business definitions to match your actual Power BI data model.

**Total Employees**
```dax
Total Employees =
DISTINCTCOUNT(Employees[EmployeeID])
```

**Active Employees**

```dax
Active Employees =
CALCULATE(
    DISTINCTCOUNT(Employees[EmployeeID]),
    Employees[EmploymentStatus] = "Active"
)
```

**Average Salary**

```dax
Average Salary =
AVERAGE(Employees[Salary])
```

**Attrition Count**

```dax
Attrition Count =
CALCULATE(
    DISTINCTCOUNT(Employees[EmployeeID]),
    Employees[EmploymentStatus] = "Resigned"
)
```

**Attrition Rate**

```dax
Attrition Rate =
DIVIDE(
    [Attrition Count],
    [Total Employees],
    0
)
```

Format the attrition rate measure as a percentage in Power BI.

**Important:** These are example measures, not verified formulas from the current dashboard. If your model records terminated employees separately, or uses a dedicated attrition flag, adjust the definitions accordingly. Confirm the denominator and reporting period used for the attrition rate before comparing it with the displayed 11%.

## 📂 Suggested Repository Structure

```text
NovaPeople-HR-Analytics/
│
├── README.md
│
├── images/
│   └── hr-analytics-dashboard.png
│
├── dashboard/
│   └── NovaPeople_HR_Analytics.pbix
│
├── data/
│   └── README.md
│
└── LICENSE
```

*This is a suggested structure. Include the folders and files that you actually publish. If the dataset is confidential, licensed, or not yours to redistribute, do not upload it; document its origin and access requirements instead.*

## 🚀 How to Use the Project

1. Clone or download this repository.
2. Open the `.pbix` file using Microsoft Power BI Desktop.
3. If the report depends on an external dataset, configure the appropriate data source and refresh the data.
4. Review the data model, Power Query transformations, and DAX measures.
5. Use the location and designation slicers to explore different workforce segments.
6. Interact with the report visuals to investigate hiring, attendance, attrition, salary, and performance patterns.

**Requirements:** Microsoft Power BI Desktop and access to any required data sources.

## 💡 Potential Business Applications

This dashboard demonstrates how HR analytics can support:

- Workforce planning and headcount monitoring.
- Identification of departments with comparatively high employee attrition.
- Exploration of employee departure reasons.
- Compensation and salary-band analysis.
- Attendance monitoring.
- Performance distribution analysis.
- Location- and designation-level workforce comparisons.

These are potential applications of the dashboard. Actual business conclusions require validation against the underlying dataset and appropriate business context.

## 📚 Skills Demonstrated

- Power BI report development.
- Power Query data transformation and ETL.
- DAX measures and KPI calculations.
- Data modeling and analytical thinking.
- Interactive slicer configuration.
- HR metrics and workforce analytics.
- Dashboard layout, formatting, and visual storytelling.
- GitHub documentation and project presentation.

## 🔮 Future Improvements

- Add monthly and yearly workforce trend analysis.
- Develop drill-through pages for department-level analysis.
- Introduce employee tenure and retention metrics.
- Add a dedicated recruitment funnel and time-to-hire analysis.
- Implement dynamic titles and KPI comparisons against previous periods.
- Improve accessibility, tooltips, and mobile report layouts.
- Add a documented data dictionary and DAX measure reference.
- Validate all measures against a defined HR reporting methodology.

## 👤 Author

**Your Name**

Aspiring Data Analyst | Power BI | SQL | Excel | Data Analytics

- GitHub: [Your GitHub Profile](https://github.com/your-username)
- LinkedIn: [Your LinkedIn Profile](https://www.linkedin.com/in/your-profile/)

*Replace the example profile links with your actual profile URLs.*

## 📄 License

This project is intended for educational, portfolio, and demonstration purposes. Add an appropriate open-source license only if you have the rights to license all included project materials. Otherwise, specify the applicable ownership and usage terms.

---

⭐ If you find this project useful or interesting, feel free to explore the repository and share your feedback.

**Disclaimer:** NovaPeople HR Solutions and the associated HR analytics scenario are hypothetical. Dashboard values and business interpretations should be treated as illustrative unless independently validated against the actual project dataset.
