# ORM Challenge 
This repository includes a fully functional backend for an e-commerce application built with Express.js and Sequelize. Below is an overview of the implemented features and functionalities:

Model Definitions
Category: Represents product categories, with a one-to-many relationship with products.
Product: Represents individual products, with fields for product name, price, stock, and associations with categories and tags.
ProductTag: A join table for the many-to-many relationship between products and tags.
Tag: Represents product tags, with a many-to-many relationship with products.

API Routes
Categories:
GET /api/categories: Retrieve all categories, including associated products.
GET /api/categories/:id: Retrieve a single category by ID, including associated products.
POST /api/categories: Create a new category.
PUT /api/categories/:id: Update a category by ID.
DELETE /api/categories/:id: Delete a category by ID.

Products:
GET /api/products: Retrieve all products, including associated categories and tags.
GET /api/products/:id: Retrieve a single product by ID, including associated categories and tags.
POST /api/products: Create a new product with optional tag associations.
PUT /api/products/:id: Update a product by ID, including tag associations.
DELETE /api/products/:id: Delete a product by ID.

Tags:
GET /api/tags: Retrieve all tags, including associated products.
GET /api/tags/:id: Retrieve a single tag by ID, including associated products.
POST /api/tags: Create a new tag.
PUT /api/tags/:id: Update a tag by ID.
DELETE /api/tags/:id: Delete a tag by ID.

Database Connection
connection.js: Configures Sequelize to connect to a PostgreSQL database using environment variables for credentials and URL.
Server Initialization
server.js: Sets up the Express.js server and syncs Sequelize models to the database on startup.

Database Seeding
Utilized seeding functionality to populate the database with initial test data.
Walkthrough Video
A detailed walkthrough video is available, demonstrating:
## video : 
https://drive.google.com/file/d/1bxy9OEcoN-P40rt2WFwlF1D38MEw1jwH/view?usp=sharing

How to create the schema from the PostgreSQL shell.
How to seed the database from the command line.
How to start the application server.
Testing GET routes for categories, products, and tags in Insomnia.
Testing POST, PUT, and DELETE routes for categories, products, and tags in Insomnia.





## screenshot:
![image](https://github.com/user-attachments/assets/d1342926-e1b4-4b2e-b160-d8988c198ad5)
![image](https://github.com/user-attachments/assets/532285dd-73c8-4001-a733-2fb36d1c8940)





