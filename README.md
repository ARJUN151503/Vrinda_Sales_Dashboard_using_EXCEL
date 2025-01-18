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
  ### Note: To Create the new column use *"shift + Alt + I + C"* if it not work use *"Alt + I + C"*
- As per taken Above sample questions shows the highest sales in months?
- So Again inserting new column named as "Month" that shows the "Month Name"
- Use Text(Values,Format_text) function --> =TEXT(G2,"mmmm") # using "mmm" it shows "JAN", using "mmmm" shows "January" use as per your work.
- 
