# Student Performance Dashboard

**Academic & Behavioral Insights**

## Project Overview

The **Student Performance Dashboard** is an interactive Power BI report designed to analyze and visualize students’ academic performance, attendance, and behavioral patterns across different classes, subjects, and terms.

The objective of this dashboard is to provide a clear, data-driven overview that helps in identifying trends, strengths, and areas of improvement for students.

---

## Dataset Description

The dashboard is built using four datasets:

### 1. Students

Contains basic student information:

* StudentID
* Name
* Gender
* Class
* Section

### 2. Scores

Contains academic performance details:

* StudentID
* Subject
* ExamType
* Score
* MaxScore
* Term

### 3. Attendance

Tracks student attendance:

* StudentID
* Date
* Status (Present/Absent)
* Reason

### 4. Behavior

Records behavioral observations:

* StudentID
* Date
* BehaviorType
* Notes

---

## Data Modeling

* All datasets were loaded into Power BI.
* Relationships were created using **StudentID** as the primary key.
* The **Students** table acts as the central dimension table.
* Data types were corrected and null values handled where required.

---

## DAX Measures Created

The following calculated measures were implemented:

1. **% Score**

   * Score divided by MaxScore.

2. **Average Score per Subject**

   * Average academic performance across subjects.

3. **Attendance %**

   * Ratio of present days to total attendance records.

4. **Behavior Count per Type**

   * Total occurrences of each behavior category.

5. **Performance Category**

   * Categorized as:

     * High (≥80%)
     * Medium (40%–79%)
     * Low (<40%)

6. **KPI Measures**

   * Total Students
   * Average Attendance
   * Average Overall Score
   * Behavior Count

---

## Dashboard Visualizations

The report includes the following visuals:

### KPI Cards

* Total Students
* Average Attendance
* Average Score
* Behavior Count

### Charts

* **Bar Chart:** Average score by Subject and Class
* **Line Chart:** Performance trend by Term
* **Donut Chart:** Behavior type distribution

### Table

* Student-wise performance details
* Conditional formatting:

  * Green: Score > 80%
  * Red: Score < 40%

---

## Interactivity Features

* Slicers for:

  * Class
  * Section
  * Subject
  * Term
* Drillthrough page for individual student profiles.
* Dynamic filtering across all visuals.

---

## Key Insights

* Overall student performance trends across terms can be easily identified.
* Subjects with higher or lower average scores are clearly visible.
* Attendance patterns help correlate performance with presence.
* Behavioral trends highlight positive and negative student conduct.

---

## Tools Used

* **Power BI Desktop**
* DAX (Data Analysis Expressions)
* Power Query for data cleaning

---

## Deliverable

* Power BI report file: `Student_Performance_Dashboard.pbix`

---

## Conclusion

This dashboard provides a comprehensive and interactive overview of student performance by combining academic, attendance, and behavioral data. It enables quick analysis, better decision-making, and improved understanding of student outcomes.
