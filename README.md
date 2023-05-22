# PowerBI-case-study
This repository is showing my previous PowerBI Case study dashboard files

## Task 5
The task 5 is to create a dashboard that looks aesthetically pleasing. Files can be located in Section Five Data Extracts, please import all columns from the excel file.
The dashboard should contain:
1. Header, background color to be #101D42
2. Slicer with Colors from dim_Product, to be placed inside the Header
3. Measures table (using DAX) with measures for Products Sold, Total Customers, Total Sales Amount
4. Three boxes to show Total Sales Amount, Products Sold and Amount of Customers. Each box should have the same background color as the Header, and also contain an image (images can be found in 5.Report Designer - 3. Icons). The values need to be shown inside the card visual. Boxes, images and values need to be aligned accordingly, values’ font size should be increased.
5. Two boxes with the same background color as Header. The first box should contain a donut chart showing the split between Male and Female, switch off the title from the donut chart and use Text Box. The text inside Text Box should say “Total Products Sold Male/Female Split”, font size to be bold, 24px, color to be #DB162F . Donut labels should be increased to 14 px. The donut colors should be white 20% Darker for Male and for Female use #DB162F. The second box should have a title called “Total Products Sold by Country”, same font size and color settings as the first box. Total products sold by country should be displayed using a bar chart. Title should be switched off from the bar chart, font size should be increased on both y and x axis.

## Task 6
1. Import all five tables from the Excel File called “Section Six Data Extract” into Power Query Mode
2. Create “Username” column inside dim_Customer table from the email address column. We are only looking for the text before the “@” symbol. The column should also be labeled “Username”
3. Scan the dim_Customer table and look out for columns with lots of Null values and remove them from the table
4. Import the tables into the model and check the connections between tables, make sure that every table is connected
5. Create #Measures table using DAX
6. Create dim_Date table using “fact_InternetSales[ShipDate]” column and create the following columns “Year”, “Month”, “Month Name”, “Day of Week”, “Quarter”, “Year/Quarter”. Make sure that the Month column is sorted correctly
7. Dynamic measure for selected currency, based on the selected currency the measure should return the sales amount in the selected currency, if no currency has been selected the measure should say “No currency selected”.
8. Dynamic measure for title that should say “Sales Amount in [Selected Currency] vs All Currencies“, alternatively it should say “Please Select Currency from the Dropdown Menu”
9. Create measures for Previous One Month, Previous Three Months and Previous Six Months
10. Measure that will tell us the time the report was last opened, text should say “Executed: Date and Time”
11. Header (background color optional) with line color #e8d400
12. Insert logo (located inside 3.Images) inside the header and resize it accordingly
13. Create buttons for “Clear Filters” (apply red outline on this button only), “Users” (apply outline using color #e8d400 on the rest of the buttons), “Currency”, “Sales Territory”. Buttons need to be positioned inside the header
14. Executed Measure to be placed inside the header on the right using Card Visual and resized accordingly, text should be on one line.
15. Create dropdown menus using bookmarks for Users, Currency and Sales Territory. The dropdown menus should have outline color of #e8d400 and an arrow pointing up to close the menu(arrow can be located inside 3.Images). Each of the dropdowns should contain the option to search inside the filter.
16. Create a bookmark that clears all the filters and apply it to “Clear Filters” button
17. Import Timeline Slicer into the visualisations panel. The visual can be located inside 4.Custom Visual. The slicer should be positioned below the header. Change the selected cells color to #e8d400
18. Create three boxes – first one to show Sales Amount in Selected Currency, second one to show Sales Amount for All Currencies in Previous Month, Sales Amount for All Time for All Currencies. Each box should have the same outline color of #e8d400. Text should be aligned in the middle, font size to be increased based on user preference. Sales Amount for Last Month and Sales Amount for All Time should not be filtered when choosing currency or region from the Header menu.
19. *Find out how to Increase Canvas Size to 1720h x 1280w
20. Position the Dynamic Title Measure in the middle inside a card visual with appropriate font size.
21. Using Line and stacked column chart create a visual that shows all Sales Amount in All Currencies, split by month name. Bar color to be #293537. Font size to be increased accordingly. *Inside the chart we should show the selected currency from the dropdown menu as a dot. Marker size to be 10 pixels. The dot color should be #e8d400. The chart should also have a Legend. Legend to be positioned in Top Center. Data lables should be visible for the bars, but not for the dots. The visual should have a placeholder in the background with line color #e8d400
22. Additional Dynamic Title Measure to be created. This title should tell us Total Products sold in the selected country or alternatively Total Products Sold Worldwide. This should be triggered by the Sales Territory Dropdown button from the Header
23. Number of Products Sold by Country to be shown inside a map visual. Change the color of the country to #e8d400. The visual should have a placeholder in the background with line color #e8d400
24. Create a table that shows the SalesTerritory along with the Sales Amount as %, Total Sales Amount, Sales for Previous One Month, Previous Three Months, Previous Six Months. Font size to be increased accordingly, outline to be removed. Column headers to be colored in #e8d400. Totals should have the same background color as per headers. Remove the outline from Totals as well. SalesTerritoryCountry background color to be changed to the same color as Totals. All headers should be capitalised. Apply conditional formatting to the Total Sales Amount %. If values are between 0 and less than or equal to 0.2 make it red, if it is greater than or equal to 0.3 and less than 0.5, make it #e8d400, if it is greater than or equal to 0.5 and less than or equal to 1, make it green
25. Test out the dashboard, make sure that everything works in sync. Bonus points if you can figure out how to change the boxes inside the Currency dropdown from a box to “Single Select” so that users can only choose one Currency from the dropdown menu at a time.
