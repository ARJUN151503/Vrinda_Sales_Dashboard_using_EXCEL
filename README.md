# Vrinda Sales Dashboard using EXCEL

## Objective

- Vrinda Store wants to create an annual sales report for 2022. So that,Vrinda can understand their customers and grow more sales in 2023.

- dataset link: [Vrinda Store Data Analysis.xlsx](https://github.com/user-attachments/files/18464177/Vrinda.Store.Data.Analysis.xlsx)

## Sample Questions

1. Compare the sales and orders using single chart.
2. Which month got the highest sales and orders ?
3. Who purchase more *"Men" or "Women"* in 2022?
4. What are the different order status in 2022?
5. List top 10 states Contributing to the sales?
6. Relation between age and gender based on number of orders.
7. Which channel is contributing to maximum sales?
8. Highest Selling Category? etc...

## Data Cleaning

- Open the Dataset and observe the coulmns and rows to undertand.
- Apply filters for all columns. Go to Data >> Filter >> click it.
- In first and second column doesn't have any unknown or improper data.
- But in third column it has *" M, W, Men, Women "*. To change it into either char like *"M and W"* or *"Men and Women"*.
- Filter the gender column by selecting *M* and open find and replace using CTRL + F and click on replace replace with *Men* and do same for *Women* also.
- Next check each and every column for any cleaning occurs.
- At *Qty* column contains *One and Two* instead of 1,2,3... .So, do the same procedure for the this column also.
- Finally, all the remaining columns are well and no inconsistance data occured. So, Our data cleaning is Done 🎉🎉 

## Data Preprocessing

- This one of important step for data
- Now in dataset insert extra column as *"Age Group"* after age column that shows the who are *"senior,Adult or Teenager"*
- By using Nested IF() or IF() function --> =IF(E2>=50,"Senior",IF(E2>=30,"Adult","Teenager"))
- As per taken Above sample questions shows the highest sales in months?
- So Again inserting new column named as "Month" that shows the "Month Name"
- Use Text(Values,Format_text) function --> =TEXT(G2,"mmmm") # using "mmm" it shows "JAN", using "mmmm" shows "January" use as per your work.
- After check all the data its enough for preprocessing if need make more than above but as per requirements its done🎊🎊.

## Data Analysis

- First Create a Pivot table. In a new sheet it appears with PivotTable Fields and blank Pivot
- Now Drag and drop the columns "Amount","orderID" in values and "Month" in Rows. Make sure that Amount should be in "SUM" and OrderId in "Count".
- Here "Total sales" need so taken "Sum of Amount".
- Then the pivot table look like this:
    ![Pivot Table 1](https://github.com/user-attachments/assets/e7592660-2ef4-46bb-9d6f-dd642b4f1616)
- Now create a pivot chart based on the pivot table.
  #### Combo Chart:
  Here based on pivot table using pivot combo chart. Steps follows:
  1. First any where on pivot table.
  2. Click on the PivotTableAnalyze tab.
  3. click on pivotchart >> Insert chart pop-up display >> click on combo chart.
  4. When select combo chart, custom combination will display. There enable the Secondary axis check box for Count of order ID and click Ok.
  5. Now combo chart is displayed.
  6. To remove column names in chart, Go to PivotChart Analyze tab >> click on Field Buttons >> click hide all. (If want make some changes....)
  7. Here the final output:
       ![Order Vs Sales by Month](https://github.com/user-attachments/assets/2aebd22f-a5c1-48ab-8841-6e9183b69719)

  

