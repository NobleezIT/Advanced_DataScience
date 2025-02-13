### **Sorting, Filtering, and Data Validation in Excel**  
*(Essential skills for organizing and managing data in analytics)*  

---

### **1. Sorting Data**  
Sorting organizes data in ascending/descending order or custom rules.  

#### **a. Basic Sorting**  
1. **Single Column Sort**:  
   - Select a cell in the column → *Data → Sort A to Z* (ascending) or *Sort Z to A* (descending).  
   - **Shortcut**: Right-click → *Sort*.  
   - **Example**: Sort a "Sales" column from highest to lowest.  

2. **Multi-Column Sort**:  
   - Go to *Data → Sort*.  
   - Add levels (e.g., first sort by "Region", then by "Sales" descending).  
   - Check *My data has headers* to exclude headers from sorting.  

#### **b. Custom Sort**  
- Sort by cell color, font color, or custom lists (e.g., days of the week).  
- **Example**: Sort by a custom list: `Low, Medium, High`.  

#### **c. Common Mistakes**  
- Sorting partial ranges (always select the entire dataset).  
- Forgetting to expand selections, causing mismatched rows.  

---

### **2. Filtering Data**  
Filtering displays only rows that meet specific criteria.  

#### **a. Basic Filters**  
1. **Apply a Filter**:  
   - Select the dataset → *Data → Filter* (or `Ctrl` + `Shift` + `L`).  
   - Click the dropdown arrow in the header to set criteria.  

2. **Filter Types**:  
   - **Text Filters**: Equals, contains, begins with.  
   - **Number Filters**: Greater than, top 10, between.  
   - **Date Filters**: Before, after, this week.  

#### **b. Advanced Filters**  
- Use *Data → Advanced Filter* to apply complex criteria (e.g., filter rows where "Sales > 1000" AND "Region = East").  
- **Example**:  
  ```  
  Criteria Range:  
  | Sales | Region |  
  | >1000 | East   |  
  ```  

#### **c. Wildcards in Filters**  
- `*` (any number of characters) and `?` (single character).  
- **Example**: Filter text starting with "A": `A*`.  

#### **d. Clear Filters**  
- Click *Data → Clear* or the filter dropdown → *Clear Filter*.  

---

### **3. Data Validation**  
Control input to prevent errors and enforce consistency.  

#### **a. Set Up Validation Rules**  
1. **Dropdown Lists**:  
   - Select cells → *Data → Data Validation → Allow: List*.  
   - Enter comma-separated values or a range (e.g., `=A1:A5`).  
   - **Example**: Restrict "Status" to `Pending, Approved, Rejected`.  

2. **Numeric Limits**:  
   - Allow only whole numbers between 1 and 100.  

3. **Date Ranges**:  
   - Restrict dates to a specific period (e.g., >= `2023-01-01`).  

4. **Custom Formulas**:  
   - Validate using a formula (e.g., force uppercase: `=EXACT(A1, UPPER(A1))`).  

#### **b. Input Messages & Error Alerts**  
- **Input Message**: Display a hint when the cell is selected.  
- **Error Alert**: Show a warning/block invalid entries.  

#### **c. Circle Invalid Data**  
- Highlight existing errors with *Data → Data Validation → Circle Invalid Data*.  

#### **d. Limitations**  
- Data validation doesn’t apply to copied/pasted data unless revalidated.  

---

### **4. Best Practices**  
1. **Sorting**:  
   - Always include headers to avoid mixing data.  
   - Use *Undo* (`Ctrl` + `Z`) if sorting goes wrong.  
2. **Filtering**:  
   - Use *Filter by Selected Cell Value* for quick filtering.  
   - Combine with conditional formatting to highlight filtered results.  
3. **Data Validation**:  
   - Protect validated cells (*Review → Protect Sheet*) to prevent tampering.  
   - Use named ranges for dropdown lists to simplify updates.  

---

### **5. Hands-On Exercises**  
#### **Exercise 1: Sales Data Cleanup**  
1. Download [sales_data.csv](link).  
2. **Sort**: Sort by "Order Date" (oldest to newest).  
3. **Filter**: Show orders with "Quantity" > 50 and "Status" = "Shipped".  
4. **Validate**: Add a dropdown to the "Region" column with options: `North, South, East, West`.  

#### **Exercise 2: Employee Database**  
1. **Sort**: Sort by "Department" A-Z, then by "Salary" descending.  
2. **Filter**: Use a wildcard to find employees with names ending in "son".  
3. **Validate**: Restrict "Hire Date" to dates after `2000-01-01`.  

---

### **6. Quick Reference Cheat Sheet**  
| **Task**                | **Steps**                                 |  
|-------------------------|-------------------------------------------|  
| Sort by multiple columns | *Data → Sort → Add Level*                 |  
| Filter by color          | Filter dropdown → *Filter by Color*       |  
| Create a dropdown list   | *Data → Data Validation → List*           |  
| Remove duplicates        | *Data → Remove Duplicates*                |  
| Advanced Filter          | *Data → Advanced Filter*                  |  

---

### **7. Common Errors & Fixes**  
- **Headers sorted as data**: Always check *My data has headers*.  
- **Filtered data not updating**: Refresh filters after editing data.  
- **Validation ignored in formulas**: Use `IFERROR` to handle invalid inputs.  

--- 

**Downloadable Resources**:  
- [Data Validation Template](link-to-template)  
- [Practice Dataset for Sorting/Filtering](link-to-CSV)  

Master these tools to ensure your data is clean, organized, and analysis-ready! 🛠️📊