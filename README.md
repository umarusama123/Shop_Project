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
# Adds products to the inventory
product1 = Product("laptop", "Electronics", 999.99, 10, "1")
product2 = Product("hat", "Clothing", 19.99, 10, "2")
product3 = Product("cola", "Drink",2.49,10,"3")
inventory.add_product(product1)
inventory.add_product(product2)
inventory.add_product(product3)
# Gets information about a product

report.print_products()


Results
"
Product Report:
Name: laptop
Category: Electronics
Price: 999.99        
Quantity: 10

Name: hat
Category: Clothing   
Price: 19.99
Quantity: 10

Name: cola
Category: Drink      
Price: 2.49
Quantity: 10
"






print("get info")
inventory.get_info("2")

get info
Name: hat
Category: Clothing
Price: 19.99
Quantity: 10
ID: 2




inventory.subtract_prod("3")
report.print_products()

Result"
Product Report:
Name: laptop
Category: Electronics
Price: 999.99
Quantity: 10

Name: hat
Category: Clothing
Price: 19.99
Quantity: 10
"



# Create a sale
sale1 = Sale(product1, 2)
sale2 = Sale(product2, 3)

# Create a transaction and add the sales

transaction.add_sale(sale1)
transaction.add_sale(sale2)

# Calculate the total amount of the transaction
total_amount = transaction.total_amount()

# Print the sales report
report.print_sales()
print(f"Total Earned:{total_amount}")
print()
# Print the product report
report.print_products()


Output
Sales Report:
Product: laptop
Quantity: 2
Price: 999.99

Product: hat
Quantity: 3
Price: 19.99

Total Earned:2059.95

Product Report:
Name: laptop
Category: Electronics
Price: 999.99
Quantity: 8

Name: hat
Category: Clothing
Price: 19.99
Quantity: 7
