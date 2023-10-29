# Shop_Project
*Shop project for project1
<br />Project Report:
<br />Implemented functions
<br />product class that creates and stores products
<br />inventory class that creates and stores inventories
<br />Sale class that creates and stores sales
<br />Transactions class that stores all sales and transactions as well as updating numbers to reflect the occured sales
<br />Report class that prints all sales and products in inventory
<br />Tracks all individual sales, as well as total earned




# Test results are below

# Product and inventory
## Adds products to the inventory
<br />product1 = Product("laptop", "Electronics", 999.99, 10, "1")
<br />product2 = Product("hat", "Clothing", 19.99, 10, "2")
<br />product3 = Product("cola", "Drink",2.49,10,"3")
<br />inventory.add_product(product1)
<br />inventory.add_product(product2)
<br />inventory.add_product(product3)
report.print_products()
## Results 1
<br />Product Report:
<br />Name: laptop
<br />Category: Electronics
<br />Price: 999.99        
<br />Quantity: 10
<br />
<br />Name: hat
<br />Category: Clothing   
<br />Price: 19.99
<br />Quantity: 10
<br />
<br />Name: cola
<br />Category: Drink      
<br />Price: 2.49
<br />Quantity: 10





## Gets info of specific product
<br />print("get info")
<br />inventory.get_info("2")

## Result 2
<br />Name: hat
<br />Category: Clothing
<br />Price: 19.99
<br />Quantity: 10
<br />ID: 2



## Subtracts product 
<br />inventory.subtract_prod("3")
<br />report.print_products()

## Result 3
<br />Product Report:
<br />Name: laptop
<br />Category: Electronics
<br />Price: 999.99
<br />Quantity: 10

<br />Name: hat
<br />Category: Clothing
<br />Price: 19.99
<br />Quantity: 10


# Sales and transactions
## Creates sales
<br />sale1 = Sale(product1, 2)
<br />sale2 = Sale(product2, 3)

## Create a transaction and add the sales

<br />transaction.add_sale(sale1)
<br />transaction.add_sale(sale2)

## Calculate the total amount of the transaction
<br />total_amount = transaction.total_amount()

## Print the sales report
<br />report.print_sales()
<br />print(f"Total Earned:{total_amount}")
<br />print()
<br />## Print the product report
<br />report.print_products()

## Result 3
<br />Output
<br />Sales Report:
<br />Product: laptop
<br />Quantity: 2
<br />Price: 999.99

<br />Product: hat
<br />Quantity: 3
<br />Price: 19.99

<br />Total Earned:2059.95

<br />Product Report:
<br />Name: laptop
<br />Category: Electronics
<br />Price: 999.99
<br />Quantity: 8

<br />Name: hat
<br />Category: Clothing
<br />Price: 19.99
<br />Quantity: 7
