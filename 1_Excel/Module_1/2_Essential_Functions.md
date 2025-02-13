### **Essential Excel Functions for Data Analytics**  
Master these core functions to clean, analyze, and visualize data efficiently.  

---

#### **1. Core Math & Statistical Functions**  
**a. `SUM`**  
- **Purpose**: Add values in a range.  
- **Syntax**: `=SUM(number1, [number2], ...)`  
- **Example**:  
  ```  
  =SUM(A1:A10) → Adds all values from cells A1 to A10.  
  ```  

**b. `AVERAGE`**  
- **Purpose**: Calculate the mean of a range.  
- **Syntax**: `=AVERAGE(number1, [number2], ...)`  
- **Example**:  
  ```  
  =AVERAGE(B2:B20) → Computes average sales in B2:B20.  
  ```  

**c. `COUNT` / `COUNTA`**  
- **Purpose**:  
  - `COUNT`: Count cells with numbers.  
  - `COUNTA`: Count non-empty cells.  
- **Syntax**:  
  ```  
  =COUNT(A1:A10)  
  =COUNTA(A1:A10)  
  ```  

**d. `MIN` / `MAX`**  
- **Purpose**: Find the smallest or largest value in a range.  
- **Syntax**:  
  ```  
  =MIN(A1:A100)  
  =MAX(A1:A100)  
  ```  

**e. `SUMIF` / `SUMIFS`**  
- **Purpose**: Sum values based on criteria.  
  - `SUMIF`: Single criterion.  
  - `SUMIFS`: Multiple criteria.  
- **Syntax**:  
  ```  
  =SUMIF(range, criteria, [sum_range])  
  =SUMIFS(sum_range, criteria_range1, criteria1, [criteria_range2, criteria2], ...)  
  ```  
- **Example**:  
  ```  
  =SUMIFS(Sales, Region, "East", Product, "Widget") → Sum sales of "Widget" in the "East" region.  
  ```  

---

#### **2. Text Functions**  
**a. `CONCATENATE` / `TEXTJOIN`**  
- **Purpose**: Combine text from multiple cells.  
  - `TEXTJOIN` includes a delimiter (Excel 2016+).  
- **Syntax**:  
  ```  
  =CONCATENATE(A1, " ", B1) → Joins A1 and B1 with a space.  
  =TEXTJOIN(", ", TRUE, A1:A10) → Joins A1:A10 with commas, ignoring blanks.  
  ```  

**b. `LEFT` / `RIGHT` / `MID`**  
- **Purpose**: Extract parts of a text string.  
- **Syntax**:  
  ```  
  =LEFT(text, [num_chars])  
  =RIGHT(text, [num_chars])  
  =MID(text, start_num, num_chars)  
  ```  
- **Example**:  
  ```  
  =MID(A1, 3, 5) → Extracts 5 characters starting at the 3rd position in A1.  
  ```  

**c. `TRIM`**  
- **Purpose**: Remove extra spaces from text.  
- **Syntax**: `=TRIM(A1)`  

**d. `SUBSTITUTE`**  
- **Purpose**: Replace specific text in a string.  
- **Syntax**: `=SUBSTITUTE(A1, "old_text", "new_text")`  

---

#### **3. Lookup & Reference Functions**  
**a. `VLOOKUP`**  
- **Purpose**: Look up values vertically in a table.  
- **Syntax**:  
  ```  
  =VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])  
  ```  
- **Example**:  
  ```  
  =VLOOKUP("Widget", A1:D100, 3, FALSE) → Finds "Widget" in column A and returns the value from column 3.  
  ```  

**b. `HLOOKUP`**  
- **Purpose**: Look up values horizontally in a table.  
- **Syntax**: Similar to `VLOOKUP` but for rows.  

**c. `INDEX-MATCH`**  
- **Purpose**: Flexible alternative to `VLOOKUP` (more efficient).  
- **Syntax**:  
  ```  
  =INDEX(return_range, MATCH(lookup_value, lookup_range, 0))  
  ```  
- **Example**:  
  ```  
  =INDEX(C1:C100, MATCH("Widget", A1:A100, 0)) → Finds "Widget" in column A and returns the corresponding value from column C.  
  ```  

**d. `XLOOKUP` (Excel 365+)**  
- **Purpose**: Modern replacement for `VLOOKUP`/`HLOOKUP` (simpler syntax).  
- **Syntax**:  
  ```  
  =XLOOKUP(lookup_value, lookup_array, return_array)  
  ```  

---

#### **4. Logical Functions**  
**a. `IF`**  
- **Purpose**: Return values based on a condition.  
- **Syntax**:  
  ```  
  =IF(logical_test, [value_if_true], [value_if_false])  
  ```  
- **Example**:  
  ```  
  =IF(A1 > 100, "High", "Low") → Labels values above 100 as "High".  
  ```  

**b. `IFS` (Excel 2016+)**  
- **Purpose**: Evaluate multiple conditions without nesting.  
- **Syntax**:  
  ```  
  =IFS(condition1, value1, condition2, value2, ...)  
  ```  

**c. `AND` / `OR`**  
- **Purpose**: Combine multiple conditions.  
- **Syntax**:  
  ```  
  =AND(A1 > 50, B1 < 100) → Returns TRUE if both conditions are met.  
  ```  

---

#### **5. Date & Time Functions**  
**a. `TODAY` / `NOW`**  
- **Purpose**: Insert current date or datetime.  
- **Syntax**:  
  ```  
  =TODAY() → Returns today’s date.  
  =NOW() → Returns current date and time.  
  ```  

**b. `DATEDIF`**  
- **Purpose**: Calculate the difference between two dates.  
- **Syntax**:  
  ```  
  =DATEDIF(start_date, end_date, "unit") → "unit" can be "Y" (years), "M" (months), "D" (days).  
  ```  

---

#### **6. Data Analysis Functions**  
**a. `COUNTIF` / `COUNTIFS`**  
- **Purpose**: Count cells meeting criteria.  
- **Syntax**:  
  ```  
  =COUNTIF(range, criteria)  
  =COUNTIFS(criteria_range1, criteria1, ...)  
  ```  

**b. `CORREL`**  
- **Purpose**: Calculate correlation between two datasets.  
- **Syntax**: `=CORREL(array1, array2)`  

**c. `RANK` / `RANK.EQ`**  
- **Purpose**: Rank values in a dataset.  
- **Syntax**: `=RANK(number, ref, [order])`  

---

#### **7. Advanced Functions**  
**a. `FILTER` (Excel 365+)**  
- **Purpose**: Dynamically filter data based on criteria.  
- **Syntax**:  
  ```  
  =FILTER(array, include, [if_empty])  
  ```  
- **Example**:  
  ```  
  =FILTER(A1:C100, B1:B100 > 100) → Returns rows where column B > 100.  
  ```  

**b. `UNIQUE` (Excel 365+)**  
- **Purpose**: Extract unique values from a range.  
- **Syntax**: `=UNIQUE(array)`  

**c. `IFERROR`**  
- **Purpose**: Handle errors gracefully.  
- **Syntax**:  
  ```  
  =IFERROR(formula, value_if_error)  
  ```  
- **Example**:  
  ```  
  =IFERROR(VLOOKUP(...), "Not Found") → Returns "Not Found" if lookup fails.  
  ```  

---

### **Quick Reference Cheat Sheet**  
| **Category**       | **Key Functions**                          |  
|---------------------|--------------------------------------------|  
| Math & Stats        | SUM, AVERAGE, SUMIFS, COUNTIFS             |  
| Text                | CONCATENATE, LEFT/RIGHT/MID, TRIM          |  
| Lookup              | VLOOKUP, XLOOKUP, INDEX-MATCH              |  
| Logical             | IF, IFS, AND/OR                            |  
| Date/Time           | TODAY, DATEDIF                             |  
| Advanced            | FILTER, UNIQUE, IFERROR                    |  

---

### **Hands-On Exercise**  
1. **Task**: Analyze sales data.  
   - Use `SUMIFS` to calculate total sales for "Product A" in the "West" region.  
   - Use `VLOOKUP` to find the price of a product from a price table.  
   - Clean a messy text column with `TRIM` and `SUBSTITUTE`.  

--- 

**Pro Tip**: Combine functions like `IFERROR` with `VLOOKUP` to avoid errors in your reports!  

[Practice datasets!](?) 

🔗 Explore more: [GCF Global Excel Learning](https://edu.gcfglobal.org/en/excel/)
📈
