# YuvaIntern - Virtual Data Science with Python Trainee
### Task 1: Data Acquisition, Cleaning, and Preprocessing

**Intern:** Ayush Kumar  
**Platform:** YuvaIntern  
**Dataset:** Online Retail (UCI Machine Learning Repository)

---

## Objective
To acquire a public dataset, inspect its quality, identify missing values, duplicates, invalid values and potential outliers, and prepare a documented cleaned dataset for further analysis.

---

## Dataset Information
| Attribute              | Details                          |
|------------------------|----------------------------------|
| Dataset Name           | Online Retail                    |
| Source                 | UCI Machine Learning Repository  |
| Original Size          | 541,909 rows × 8 columns         |
| Cleaned Size           | 536,641 rows × 8 columns         |
| Features               | InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country |

---

## Cleaning Steps Performed
- Loaded and inspected the raw dataset
- Identified and removed **5,268** exact duplicate rows
- Analyzed missing values (mainly in `CustomerID` and `Description`)
- Detected non-positive values in `Quantity` and `UnitPrice`
- Identified potential outliers (extreme Quantity & UnitPrice values)
- Generated cleaning summary and missing values report

---

## Files Included
| File Name                        | Description                              |
|----------------------------------|------------------------------------------|
| `Task1_Data_Cleaning.ipynb`      | Complete Jupyter Notebook with all steps |
| `task1_cleaning_summary.csv`     | Summary of cleaning operations           |
| `task1_missing_values_report.csv`| Missing values analysis                  |

---

## Key Results
- **Duplicate rows removed:** 5,268  
- **Missing values remaining:**  
  - CustomerID → 135,037 (25.16%)  
  - Description → 1,454 (0.27%)  
- **Records with Quantity ≤ 0:** 10,587  
- **Records with UnitPrice ≤ 0:** 2,512  

---

## Tools & Libraries Used
- Python 3
- Pandas
- NumPy
- Matplotlib / Seaborn

---

## How to Run
1. Open `Task1_Data_Cleaning.ipynb` in Jupyter Notebook or Google Colab
2. Ensure the original dataset (`Online Retail.xlsx`) is available
3. Run all cells sequentially
