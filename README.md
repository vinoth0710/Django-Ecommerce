# Django E-Commerce Project

This project showcases an e-commerce website built with Django. It includes models for products, promotions, customers, orders, and more. The structure consists of main app files, a management script, and a requirements file. 

## Features

- Manage products, promotions, and collections
- Handle customer orders, addresses, and carts
- Explore the admin panel for easy management
- Built using Django's powerful web framework
- Clone, install dependencies, and run the server to start

## Usage

1. Clone the repository.
2. Set up a virtual environment and install dependencies.
3. Apply migrations and create a superuser.
4. Run the development server.
5. Access the admin panel at `/admin/`.

Feel free to contribute or customize for your own e-commerce needs.


Models create in this E commerce Project

Promotion
+----+----------------+---------+
| ID | Description    | Discount|
+----+----------------+---------+

Collection
+----+----------------+-----------------+
| ID | Title          | Featured Product|
+----+----------------+-----------------+

Product
+----+---------+--------+------------+-----------+------------------+----------------+
| ID | Title   | Slug   | Description| Unit Price| Inventory        | Last Update    |
+----+---------+--------+------------+-----------+------------------+----------------+

Customer
+----+-----------+-----------+------------------+--------+
| ID | First Name| Last Name | Email            | Phone  |
+----+-----------+-----------+------------------+--------+

Order
+----+-----------------+---------------------+---------------+
| ID | Payment Status | Placed At           | Customer      |
+----+-----------------+---------------------+---------------+

Order Item
+----+--------+---------+----------+
| ID | Order  | Product | Quantity |
+----+--------+---------+----------+

Address
+----+---------+--------+---------+
| ID | Street  | City   | Customer|
+----+---------+--------+---------+

Cart
+----+-------------+
| ID | Created At  |
+----+-------------+

Cart Item
+----+------+---------+
| ID | Cart | Product |
+----+------+---------+
