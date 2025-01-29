# Hands-on Lab 4: Simple Use of Functions

**Estimated time needed:** 30 minutes

In this lab, first you will learn the basics of formulas, how to perform simple calculations, how to select ranges in formulas, and how to copy formulas.
Next, you will learn the basics of functions, how to use some of the more common functions that a Data Analyst might employ, and look at some of the
more advanced functions available in Excel. Finally, you will learn about referencing data in formulas; specifically how to differentiate between relative and
absolute references, and you will also learn about error handling in formulas.

# Software Used in this Lab

The instruction videos in this course use the full Excel Desktop version as this has all the available product features, but for the hands-on labs we will be
using the free ‘Excel for the web’ version as this is available to everyone.

Although you can use the Excel Desktop software if you have access to this version, it is recommended that you use Excel for the web for the hands-on labs
as the lab instructions specifically refer to this version, and there are some small differences in the interface and available features.

# Dataset Used in this Lab

The dataset used in this lab is an internal dataset.

# Objectives

After completing this lab, you will be able to:

```
Understand the basics of formulas
Perform simple calculations
Select ranges in formulas and copy formulas
Understand the basics of functions
Use common functions
Understand the more advanced functions available
Reference data in formulas
Differentiate between relative and absolute references
Understand how to handle formula errors
```
# Exercise 1: Basics of Formulas

In this exercise, you will learn the basics of formulas, how to perform simple calculations, how to select ranges in formulas, and how to copy formulas.

1. Download the file **Personal_Monthly_Expenditure_Lab4.xlsx**. Upload and open it using Excel for the web. Go to the **Expense - 2018** worksheet.


2. In **A14** , type **Totals** and in **B14** , type **=SUM(** then select cells **B2 to B13** with the mouse, and press **Enter**.
3. Select the **fill handle** on cell **B14** and drag to **G14** to copy the formula.
3. In cell **H1** , type **Monthly Total** and double-click the divider between **H and I**.
4. In **H2** , type **=SUM(** then select cells **B2 to G2** with the mouse, and press **Enter**. If necessary, select the **fill handle** on cell **H2** and drag to **H14** to
    copy the formula.
5. Select columns **B to H**. On the **Home** tab, in the **Number** group, click the **Accounting Number Format ($)** drop-down list, and select **$ English**
    **(United States)**.

# Exercise 2: Basics of Functions

In this exercise, you will have an introduction to functions, including using some common statistical functions, and then you will learn about some more
advanced functions that a Data Analyst might also use.

1. In cells **A16-A20** , type the following:

```
Avg
Min
Max
Count
Median
```
2. In **B16** , type **=AVERAGE(** then select cells **B2 to B13** with the mouse, and press **Enter**. Select the **fill handle** on cell **B16** and drag to **G16** to copy
    the formula.
3. In **B17** , type **=MIN(** then select cells **B2 to B13** with the mouse, and press **Enter**. Select the **fill handle** on cell **B17** and drag to **G17** to copy the
    formula.
4. In **B18** , type **=MAX(** then select cells **B2 to B13** with the mouse, and press **Enter**. Select the **fill handle** on cell **B18** and drag to **G18** to copy the
    formula.
5. In **B19** , type **=COUNT(** then select cells **B2 to B13** with the mouse, and press **Enter**. Select the **fill handle** on cell **B19** and drag to **G19** to copy the
    formula. Select row **19**. On the **Home** tab, click the **Number Format** drop-down list, and select **Number**.
6. In **B20** , type **=MEDIAN(** then select cells **B2 to B13** with the mouse, and press **Enter**. Select the **fill handle** on cell **B20** and drag to **G20** to copy the
    formula.


7. Explore some more commonly used functions of a data analyst by clicking the arrow under **AutoSum** , then select **More Functions** and look at some
    of the functions in various categories to see what actions they perform:
       Financial : **ACCRINT, INTRATE**
       Logical : **AND, IF, OR, NOT**
       Text : **CONCAT, FIND, SEARCH**
       Date & Time : **NETWORKDAYS, WEEKDAY**
       Lookup & Reference : **AREAS, SORTBY, VLOOKUP, HLOOKUP**
       Math & Trig : **POWER, SUMIF, SUMPRODUCT**
       Statistical : **AVERAGE, COUNTIF, MAX, MEDIAN, MIN**

# Exercise 3: Referencing Data in Formulas (relative vs absolute) &

# Formula Errors

In this exercise, you will learn how to reference data in formulas; specifically differentiating between relative and absolute references, and you will also
learn about error handling in formulas.

1. In cells **A31-A40** , type **1-10**. Select row **31 to 40**. On the **Home** tab, click the **Number Format** drop-down list, and select **General**.
2. Relative References : In cell **B33** , type **=A31+A32** and press **Enter**. Select the **fill handle** on cell **B33** and drag to **B40** to copy the formula. Here,
    both first and second cell reference will move 1 cell down. For example, on cell **B34** formula will be changed to **=A32+A33** , on cell **B35** formula will
    be changed to **=A33+A34** and so on.
3. Absolute References : In cell **C33** , type **=$A$31+$A$32** and press **Enter**. Select the **fill handle** on cell **C33** and drag to **C40** to copy the formula.
    Here, both first and second cell references will not change. For example, on cell **C34** formula will remain **=$A$31+$A$32** , on cell **C35** formula will
    remain **=$A$31+$A$32** and so on.
4. Mixed References : In cell **D33** , type **=$A$31+$A32** and press **Enter**. Select the **fill handle** on cell **D33** and drag to **D40** to copy the formula. Here,
    first cell reference will stay the same, but the second reference will change. For example, on cell **D34** formula will be changed to **=$A$31+$A33** , on
    cell **D35** formula will be changed to **=$A$31+$A34** and so on.
5. In cell **B31** , type **=A16+A17**. Now this will lead to a formula error **#VALUE!** since cells **A16** and **A17** do not contain any number.


6. Click the **question mark icon** in the error message box. This will open the **Help** for this topic. Read through this help file for more information about
    **#VALUE!** errors in formulas.

## Congratulations! You have completed Lab 4, and you are ready for the next topic.

# Author(s)

```
Sandip Saha Joy
```
# Other Contributor(s)

```
Steve Ryan
```
## © IBM Corporation 2020. All rights reserved.


