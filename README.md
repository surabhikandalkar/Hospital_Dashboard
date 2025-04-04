# Power BI Patient Waiting List Dashboard  

## 📌 Overview  
This project focuses on analyzing and visualizing patient waiting list trends (2018–2021) using Power BI. The dashboard provides insights into inpatient and outpatient wait times, specialty-level distribution, and age profile analysis.  

---

## 🚀 1. Requirement Gathering  
### 🎯 Objectives  
- Track current patient waiting list status.  
- Analyze historical trends for Inpatients & Outpatients.  
- Perform specialty & age-based analysis.  

### 📊 Data Scope  
- **Timeframe:** 2018–2021  
- **Metrics:** Avg/Median Wait List, Total Wait List  
- **Views:** Summary & Detailed Pages  

---

## 🗂️ 2. Data Collection  
### 🔗 Data Sources  
- **Excel/CSV**, **SQL Server**, **Cloud (Azure, AWS, GCP)**, **ERP (Salesforce, SAP)**  
- **Selected Source:** Folder Connection  

### 📥 Importing Data into Power BI  
1. **Get Data** → Select **Folder** → Click **Connect**  
2. Browse folder path → Click **OK**  
3. Click **Combine & Load** to import files  

---

## 🔄 3. Data Transformation  
### 🔧 Steps in Power Query Editor  
- **Rename & Rearrange Columns**  
- **Append Tables (Inpatient & Outpatient)**  
- **Clean Data (Replace, Trim, Handle Duplicates)**  

### 🔗 Data Modeling  
- **Create Relationships** (e.g., Specialty Mapping)  
- **Optimize Table Structure**  

---

## 📐 4. Visualization Blueprint  
- Wireframe design & approval before development.  

---

## 🎨 5. Dashboard Layout & Design  
### 🏗️ Setup  
- Enable **Gridlines** & **Snap to Grid** for proper alignment.  

### 📊 Key DAX Measures  
```DAX
Latest Month Wait List = CALCULATE(SUM(All_Data[Total]), All_Data[Archive_Date] = MAX(All_Data[Archive_Date])) + 0
