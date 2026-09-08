# cognevance_student-performance-analysis
# Student Performance Analysis Project

## Overview
This project aims to analyze various factors influencing student academic performance using a given dataset. Through data cleaning, exploratory data analysis, hypothesis testing, and advanced visualization techniques, key insights into student success were identified.

## Workflow

1.  **Data Loading and Preprocessing**: The `raw_student_data.csv` dataset was loaded. Missing values in numerical columns were imputed using the mean. Duplicate entries were identified and removed. The `test_preparation` column was cleaned by standardizing text and filling missing values with 'Not Reported'.
2.  **Exploratory Data Analysis (EDA) and Hypothesis Testing**: Several hypotheses were formulated and tested to understand relationships between different student attributes (e.g., attendance, study hours, parental education, gender, grade, subject) and their marks.
3.  **Advanced EDA Techniques**: 
    *   **Multi-level Segmentation**: Students were grouped by 'attendance % bucket' and 'study hours per week bucket' to analyze average marks across these segments.
    *   **Correlation Analysis**: The correlation between 'marks' and 'attendance %' was calculated to quantify their relationship.
    *   **Outlier Detection**: The IQR method was applied to identify extreme values in the 'marks' column.
4.  **Visualization**: Individual plots (bar charts, heatmaps, scatter plots with regression lines) were created to illustrate specific findings. A final 2x2 dashboard was then generated to consolidate the most impactful visualizations.
5.  **Data Narrative**: A structured data narrative (using the SCR framework) was developed to explain the project's key findings and provide actionable recommendations.

## Tools Used

*   **Python**: The primary programming language for data analysis.
*   **Pandas**: Utilized for data manipulation, cleaning, and aggregation.
*   **NumPy**: Used for numerical operations, especially with statistical calculations.
*   **Matplotlib**: Employed for creating static, interactive, and animated visualizations.
*   **Seaborn**: Used for drawing attractive and informative statistical graphics.

## Key Findings

Based on the analysis, the following key findings were observed:

*   **Attendance and Marks**: Students who fall into higher attendance buckets consistently tend to score higher overall average marks. A moderate positive correlation of 0.37 was found between attendance percentage and marks.
*   **Study Hours and Marks**: Study hours per week are almost directly proportional to marks, indicating a strong positive relationship.
*   **Combined Impact of Attendance and Study Hours**: Students attending 70%-90% of classes and studying 6-8 hours per week achieved the highest average marks (90.69). Conversely, students with 50-70% attendance and 0-2 hours of study per week had the lowest average marks (68.14).
*   **Test Preparation**: Students with 'Occasional' and 'Not Reported' test preparation types showed slightly higher average marks compared to those with 'Regular' preparation.
*   **Parental Education, Gender, and Grade**: No significant effect on student marks was observed from parental education, gender, or grade level.

These findings suggest that attendance and consistent study habits are critical determinants of student performance.
