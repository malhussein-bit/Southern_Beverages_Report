 # Southern_Beverages_Report
  Sales Performance , Product and Customer Profile of  a Multi National Beverages company in the United states 

## Tools and Technology
    - Microsoft Excel - 8 CSV Files :5 Dimension Tables :Customers, Products, Stores, Regions and        Calendar. 3 Fact Tables : Transactions 1997 , Transaction 1998 and Returns 1997-1998.
- Power BI Desktop – for building the interactive reports and dashboard.

## Data Connection and Workflow 
      Connected to the SouthernBeverages_Customers csv file
•	Named the table "Customers", and make sure that headers have been promoted
•	Confirmed that data types are accurate and of the correct 
•	Added a new column named "full_name" to merge the the "first_name" and "last_name" columns, separated by a space
•	Create a new column named "birth_year" to extract the year from the "birthdate" column, and format as text
•	Create a conditional column named "has_children" which equals "N" if "total_children" = 0, otherwise "Y"

    Connected to the SouthernBeverages_Products csv file
•	Name the table "Products" and made sure that headers have been promoted
•	Confirmed that data types are accurate  and of the correct type.
•	Use the statistics tools to return the number of distinct product brands, followed by distinct product names
•	Added a calculated column  named "discount_price", equal to 90% of the original retail price
•	Used the " the Group By option to calculate the average retail price by brand, and name the new column "Avg Retail Price"
•	Deleted the last applied step to return the table to its pre-grouped state
•	Replaced "null" values with zeros in both the "recyclable" and "low-fat" columns

 Connected to the SouthernBeverages_Stores csv file
•	Renamed  the table "Stores".
•	Confirmed that data types are 
•	Added a calculated column named "full_Addedress", by merging "store_city", "store_state", and "store_country", separated by a comma and space 
•	Added a calculated column named "area_code", by extracting the characters before the dash ("-") in the "store_phone" field 

Connected to the SouthernBeverages_Regions csv file
•	Renamed the table "Regions" .

Connected to the SouthernBeverages_Calendar csv file
•	Renamed the table "Calendar".
•	Used the date tools in the query editor to Added the following columns:
•	Start of Week (starting Sunday
•	Name of Day
•	Start of Month
•	Name of Month
•	Quarter of Year
•	Year

Connected to the SouthernBeverages_Returns csv file
•	Renamed the table "Return_Data" .

Added a new folder named "Southern Beverages Transactions", containing both the SouthernBeverages_Transactions_1997 and SouthernBeverages_Transactions_1998 csv files
•	Connected to the folder path.
•	Combine the files, then removed the "Source.Name" column
•	Named the table "Transaction_Data and confirmed that headers have been promoted.

## Key features & skills demonstrated

1- Using DAX Expressions, the following calculated columns have been added:
 •	In the Calendar table, added a column named "Weekend", Equals "Y" for Saturdays or Sundays (otherwise "N")
 •	In the Calendar table, added a column named "End of Month, Returns the last date of the current month for each row
 •	In the Customers table, added a column named "Current Age", Calculates current customer ages using the "birthdate" column and the TODAY() function
 •	In the Customers table, added a column named "Priority", Equals "High" for customers who own homes and have Golden membership cards (otherwise "Standard")   
 •	In the Customers table, added a column named "Short_Country", Returns the first three characters of the customer country, and converts to all uppercase 
 •	In the Customers table, added a column named "House Number", Extracts all characters/numbers before the first space in the "customer_Addedress" column 
 •	In the Products table, added a column named "Price Tier", Equals "High" if the retail price is >$3, "Mid" if the retail price is >$1, and "Low" otherwise
 •	In the Stores table, added a column named "Years_Since_Remodel", Calculates the number of years between the current date (TODAY()) and the last remodel date.




2- Created a Measure table name _Measures to make sure table stays at the top of the list, 

Using DAX Expressions, created the following Measures:
•	"Quantity Sold" and "Quantity Returned" to calculate the sum of quantity from each data table
•	 "Total Transactions" and "Total Returns" to calculate the count of rows from each data table
•	"Return Rate" to calculate the ratio of quantity returned to quantity sold.
•	"Weekend Transactions" to calculate transactions on weekends
•	"% Weekend Transactions" to calculate weekend transactions as a percentage of total transactions (format as %)
•	"All Transactions" and "All Returns" to calculate grand total transactions and returns (regardless of filter context)
•	to calculate "Total Revenue" based on transaction quantity and product retail price, and format as $ (hint: you'll need an iterator)
•	"Total Cost" based on transaction quantity and product cost, and format as 
•	"Total Profit" to calculate total revenue minus total cost, and format as $
•	"Profit Margin" by dividing total profit by total revenue calculate total revenue (format as %)
•	 "Unique Products" to calculate the number of unique product names in the Products table
•	"YTD Revenue" to calculate year-to-date total revenue.
•	"60-Day Revenue" to calculate a running revenue total over a 60-day period.
•	 "Last Month Transactions", "Last Month Revenue", "Last Month Profit", and "Last Month Returns"
•	"Revenue Target" based on a 5% lift over the previous month revenue.

.  


## Report and Dashboard Preview






## Key Insights

•	Tel Tale Brand reached 800 sales sold in Salem, USA in December closing out the year.
•	King Product has the highest return rate at a rate of 1.78 %
•	ADJ Brand drove the strongest overall profit margin (68.48%) sold in Portland USA



## Notes & privacy
- The pbix contains **no** confidential data; original dataset was anonymized


