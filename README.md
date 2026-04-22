# Global Public Debt vs GDP Analysis

## Language

- English (default)
- Español: [Ver versión en español](README_ES.md)
- 
## Project Overview
Exploratory data analysis of public debt and GDP across countries using Power BI, focused on understanding debt sustainability through the Debt-to-GDP ratio and identifying high-risk economies.  

The project delivers an interactive dashboard combining global comparisons, risk classification, and advanced visualizations.

---

## Objective
The main goal of this project is to analyze the relationship between:

- Total Public Debt
- Gross Domestic Product (GDP)
- Debt-to-GDP Ratio

To:

- Evaluate countries’ debt sustainability  
- Identify high-risk economies  
- Compare countries regardless of economic size  

---

## Data Sources
Data was obtained from public web sources:

- Public Debt by Country  
- GDP by Country (2022)  

Source: Datosmacro (Expansión)  
Data was imported into Power BI using Web connector (anonymous access).

---

## Data Preparation (Power Query)

### Public Debt Table
- Removed unnecessary columns  
- Selected relevant fields:
  - Country  
  - Total Debt  
  - Debt (% of GDP)  
  - Debt per Capita  
- Cleaned currency symbols and separators  
- Converted fields to numeric format  
- Standardized country names  

### GDP Table
- Cleaned GDP format (removed symbols and separators)  
- Removed errors and null values  
- Standardized country names  

### Data Enrichment
- Created a Country–Continent mapping table  
- Established relationships across tables using the country field  

---

## Data Model
- Relationship between Public Debt and GDP tables by country  
- Additional geographical dimension (continent)  
- Optimized structure for comparative analysis  

---

## Key Measures (DAX)

- Total Debt  
- Total GDP  
- Debt-to-GDP Ratio  
- Countries at Risk (Ratio > 100%)  

Risk classification:
- Low (< 60%)  
- Medium (60%–100%)  
- High (> 100%)  

---

## Dashboard Features

### KPIs
- Total GDP  
- Total Public Debt  
- Debt-to-GDP Ratio  
- Countries at High Risk  

### Global Analysis
- Map: Debt-to-GDP Ratio by Country  
- Scatter Plot: GDP vs Debt-to-GDP Ratio  
  (bubble size represents total debt)  

### Comparative Analysis
- Top 10 Countries by:
  - Total Debt  
  - GDP  
  - Debt-to-GDP Ratio  

### Segmentation
- Filters by:
  - Country  
  - Continent  

### Risk Distribution
- Donut chart showing countries by risk level  

### Advanced Features
- Custom tooltips comparing each country with its continental average  

---

## Key Insights

- Countries with the highest total debt are not necessarily the most at risk  
- The Debt-to-GDP ratio is the most relevant indicator of economic sustainability  
- Smaller economies can present disproportionately high debt levels  
- Debt per capita highlights the real burden on the population  
- Clear regional patterns can be observed across continents  

---

## Conclusion
Evaluating public debt requires more than analyzing absolute figures. By incorporating the Debt-to-GDP ratio, this project provides a more accurate view of economic sustainability across countries.

The dashboard enables a global, comparative perspective, helping to identify patterns, outliers, and high-risk economies through clear and intuitive visualizations.

---

## Skills Demonstrated

- Data Cleaning and Transformation (Power Query)  
- Data Modeling in Power BI  
- DAX Measures and Calculations  
- Data Visualization and Dashboard Design  
- Analytical Thinking and Insight Generation  
- Custom Tooltip Implementation  

---

## Dashboard Preview
<img width="3097" height="1747" alt="image" src="https://github.com/user-attachments/assets/74faca8d-b041-4209-8c8b-dc16a3a7e6dc" />

---

## Tools Used
- Power BI  
- Power Query  
- DAX  
