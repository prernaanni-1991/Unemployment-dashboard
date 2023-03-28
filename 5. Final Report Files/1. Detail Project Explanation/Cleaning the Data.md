![alt text](https://ineuron.ai/images/ineuron-logo.png)

# Indian Unemployement Rate Analysis

### Cleaning The Data

1. Chek and assign correct the data types of different coloumns.

2. Apply filter on each coloumn.

3. Split the date column in date, month & year using delimeter function.

4. Check the data type of date after splitting and change it to int data type.

5. Removed the date day column to make the observation simpler.

6. Rename the column if required.

7. Add a custom coloumn using the formula = Table.AddColumn(#"Renamed Columns", "Custom", each if [Month] = 1 then "Jan" else if [Month] = 2 then "Feb" else if [Month] = 3 then "Mar" else if [Month] = 4 then "Apr" else if [Month] = 5 then "May" else if [Month] = 6 then "Jun" else if [Month] = 7 then "Jul" else if [Month] = 8 then "Aug" else if [Month] = 9 then "Sep" else if [Month] = 10 then "Oct" else if [Month] = 11 then "Nov" else if [Month] = 12 then "Dec" else null, type text)

8. Merge two columns ( month & year) and then insert if required.
9. At the end, remove unnecessary column.

Now we have the data Cleaned.