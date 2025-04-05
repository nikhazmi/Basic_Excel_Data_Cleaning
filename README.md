# Basic_Excel_Data_Cleaning
Excel based data cleaning project using no-code tools

## Project Overview

### 1. Identify & Handle Missing Values
- **Applied Filters:**  
  Used Excel's filter feature to detect missing values in critical columns such as `Order ID`, `Product`, and `Total Price`.
- **Actions Taken:**  
  - **Order ID:** Deleted rows where `Order ID` was missing.
  - **Product:** Deleted rows missing the `Product` value.
  - **Total Price:** Recalculated missing `Total Price` using the formula:  
    ```
    =Quantity * Unit Price
    ```

### 2. Remove Duplicates
- **Tool Used:**  
  Excel's built-in **Remove Duplicates** feature (under the Data tab).
- **Method:**  
  Selected the `Order ID` column (or the entire row if needed) to remove duplicate records and ensure each order is unique.

### 3. Standardize Column Headers
- **Manual Renaming:**  
  Renamed headers to a consistent format (e.g., `Order ID` to `order_id`, `Customer Name` to `customer_name`).
- **Using a Helper Row:**  
  Inserted a new row and used the following formula to clean each header:
  ```excel
  =LOWER(SUBSTITUTE(TRIM(A1), " ", "_"))
