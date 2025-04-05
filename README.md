
# Excel Data Cleaning Project (No Power Query) 

This repository documents a simple and effective data cleaning workflow using **Microsoft Excel 2023**, without the use of Power Query. 
It demonstrates how basic Excel functions and tools can be leveraged to prepare raw data for analysis — perfect for beginners, students, or analysts working in environments with limited tool access.

#Badges

![Windows 11](https://img.shields.io/badge/Windows%2011-%230079d5.svg?style=for-the-badge&logo=Windows%2011&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![MIT License](https://img.shields.io/badge/License-MIT-%23007B5E.svg?style=for-the-badge&logo=MIT&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-%23000000.svg?style=for-the-badge&logo=Microsoft%20Excel&logoColor=white)
```

## Cleaning Process (Summary)

### Step 1: Remove Unnecessary Rows
- Deleted blank rows and extra headers to ensure the actual data starts from Row 2.
- Ensured only one row of headers at the top.

###  Step 2: Standardize and Rename Column Headers
- Used the formula:  
  ```excel
  =LOWER(SUBSTITUTE(TRIM(A1), " ", "_"))
  ```
  - `TRIM` removes extra spaces
  - `SUBSTITUTE` replaces spaces with underscores
  - `LOWER` converts to lowercase

- Replaced original headers with these cleaned ones using **Paste Special → Values**.

### Step 3: Remove Duplicates
- Selected the full data table
- Went to `Data` tab → `Remove Duplicates`
- Selected relevant columns (or all) and clicked OK

### Step 4: Format Data Types
- Ensured correct data formats:
  - Dates were formatted as `Short Date`
  - Numbers had 2 decimal places
  - Text columns were aligned and checked for consistency

### Step 5: Clean Data Cells
- Used formulas like:
  - `=TRIM(A2)` → Removes extra spaces in cell values
  - `=CLEAN(A2)` → Removes non-printable characters
- Used **Find & Replace** to correct common issues (e.g. replacing "N/A" with blank)

## Bonus Tips

- Used **Freeze Panes** to lock headers while scrolling.
- Applied **Filters** to columns using `Data → Filter` to explore data inconsistencies.
- Used **Conditional Formatting** to highlight outliers or errors.

## Tools Used

- Microsoft Excel 2023
- Excel formulas: `TRIM`, `SUBSTITUTE`, `LOWER`, `CLEAN`
- Excel built-in tools: Remove Duplicates, Filters, Formatting

## Outcome

- A clean, well-structured Excel file ready for:
  - Reporting
  - Visualization
  - Import into Power BI or SQL
  - Sharing with stakeholders

## How to Use This Repository

1. Clone or download the repo.
2. Open the `data/raw_data.xlsx` file to see the original state.
3. Check `docs/cleaning_steps.md` for a breakdown of steps taken.
4. Open `data/cleaned_data.xlsx` to view the final result.

---

## Author

**Nik Hazmi bin Nik Suhaimi**  
Excel-based data cleaner & business development executive  
Malaysia |  Aerospace & Investment | MBA Candidate

---

## 🗃License

This project is open-source and available under the MIT License.
