
# Step-by-Step Cleaning Process

### Step 1: Remove Unnecessary Rows
- Delete blank rows and headers.
- Ensure the actual data starts from Row 2.

### Step 2: Standardize and Rename Column Headers
- Use formula to clean and standardize header names.
  ```excel
  =LOWER(SUBSTITUTE(TRIM(A1), " ", "_"))
  ```

### Step 3: Remove Duplicates
- Go to `Data → Remove Duplicates`.
- Select columns to check and click OK.

### Step 4: Format Data Types
- Ensure dates are in Short Date format.
- Format numbers to 2 decimal places.

### Step 5: Clean Data Cells
- Use `=TRIM()` and `=CLEAN()` functions.
- Find & Replace to remove "N/A" or empty cells.
