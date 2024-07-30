# Global-Superstore-Dashboard

This is a Power BI analysis of Global SuperStore data. The dashboard/report is divided into three pages: Summary, Customer Analysis, and India Analysis. Each page includes slicers for year selection and category selection (Furniture, Office Supplies, and Technology).

## Dataset Description
This dataset has 3 tables for Orders, Persons, and Returns. 
The order table has 24 columns, and the Postel code was completely null, and an additional column was made as shipping time by using order data and shipping date. Some preprocessing was done to remove duplicates for the product name categories. Person table as to columns Person and Region. The Return table has Oder ID and Region. Power-BI relations were made between the order table and person table (with the region as key), as there were many-to-one relations, and the relation between the order and return table (with order ID as key) was as many-to-many relations. Using DAX, some extra metrics were made, such as profit ratio, India sales, Total sales, and Total count, which made visualization easier.


## Dashboard Overview
### 1. Summary Page
![Summary](https://github.com/user-attachments/assets/c8c32206-b753-471a-add7-3bc289382c76)

  
  - Sales: $12.64M (Cards)
  - Quantity: 178K (Cards)
  - Avg. Shipping Days: 3.97 (Cards)
  - Returned Orders: 1970 (Cards)

  - Top 10 Countries by Profit (Stacked Bar Chart)
    - Top Countries:
      - USA
      - China
      - India
      - UK
      - France
    
  - Sales by State (World Map)
    - Bubble Size: Represents sales from each state
  
  
  - Profit by Product Name: Top 5 products by profit (Horizontal Bar Charts)
  - Loss by Product Name: Top 5 products by loss (Horizontal Bar Charts)
  
  - Sales by Market (Donut Chart)
    - Market Share:
      - Asia Pacific: 31.98%
      - Europe: 26%
      - USCA: 18.7%
      - LATAM: 17.12%
      - Africa: 6.2%
        > The USA might have the highest sales among countries, but the Asia Pacific sales are higher.

### 2. Customer Analysis Page
![Customer Analysis](https://github.com/user-attachments/assets/619124a6-db2e-4077-a6b1-e6643a299122)


  - Customers: 17.42K (Card)
  - Customer with least no. of returns: Aaron Bergman (Card)

  
  - Top 5 Profit-Making Customers: Top 5 customers by profit (Horizontal Bar Chart)
  - Top 5 Customers by Profit Ratio: Top 5 customers by profit ratio (Horizontal Bar Chart)

  - Top Return Orders by Customer (Donut Chart)
    - Top 5 Returners

  - Customers by Market (Pie Chart)
    - Market Share:
      - Asia Pacific: 28.37%
      - Europe: 23.17%
      - LATAM: 21.26%
      - USCA: 15.4%
      - Africa: 11.8%

  - Profit Ratio by Market (Funnel)
    - Profit Ratio:
      - Europe: 13.68%
      - USCA: 12.87%
      - Africa: 11.34%
      - LATAM: 10.24%
      - Asia Pacific: 9.97%
> Though Asia Pacific has more customers and sales, Europe has high-profit ratio

  -  Sales and Number of Customers by Year (Line Bar Chart)
    - Trend: As the number of customers increases, sales also increase

### 3. India Analysis Page
![India Analysis](https://github.com/user-attachments/assets/ada8b1d0-ce8f-4578-9b1f-adfdd12ba307)

  - Customers: 493 (Card)

  - Returned Orders: 56 (Card)

  - Top 5 States by Sales (Pie Chart)
    - Top States:
      - Maharashtra (35.96%)
      - UP (24.93%)
      - Tamil Nadu (16%)
      - Karnataka (14.7%)
      - Delhi (7.78%)

  - Best Profit Making States (Horizontal Bar Charts): 
    - UP
    - Maharashtra
    - Tamil Nadu
    - Karnataka
    - Gujarat 

  - Worst Profit-Making States (Horizontal Bar Charts):
    - Assam
    - Puducherry
    - Manipur
    - Tripura
    - Chandigarh 

  - Profit Ratio by Market (Funnel Chart)
    - Top Markets:
      - Chandigarh (39.43%)
      - J&K (35.69%)
      - Tripura (35.21%)
      - Jharkhand (33.18%)
      - Karnataka (29.21%)
 > Though Chandigarh is worst in making a profit but has a high-profit ratio with more focus, the company can increase profits

  - Number of Customers and Sales (Line Chart)
    - Trend: As  customers increase, sales increase
      > But both graphs overlap, indicating that old customers are purchasing the same amount and are not increasing their purchase volume.
  
  - Sales and Number of Customers in India (Map)
    - Bubble Size: Represents sales in each state of India
