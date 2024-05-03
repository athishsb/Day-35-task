# MongoDB Day 1

This repository contains MongoDB queries and screenshots for various tasks related to querying a MongoDB database.

## MongoDB Queries

1. **Find all the information about each product:**
   - MongoDB Query: `db.product.find()`

2. **Find the product price which are between 400 to 800:**
   - MongoDB Query: `db.product.find({product_price: {$gt:400,$lt:800}})`

3. **Find the product price which are not between 400 to 600:**
   - MongoDB Query: `db.product.find({product_price:{$not:{$gte:400,$lte:600}}})`

4. **List the four products which are greater than 500 in price:**
   - MongoDB Query: `db.product.find({product_price:{$gt:500}}).limit(4)`

5. **Find the product name and product material of each product:**
   - MongoDB Query: `db.product.find().projection({product_name:1,product_material:1})`

6. **Find the product with a row id of 10:**
   - MongoDB Query: `db.product.find({id:"10"})`

7. **Find only the product name and product material:**
   - MongoDB Query: `db.product.find().projection({_id:0,product_name:1,product_material:1})`

8. **Find all products which contain the value 'soft' in product material:**
   - MongoDB Query: `db.product.find({product_material:"Soft"})`

9. **Find products which contain product color 'indigo' and product price 492:**
   - MongoDB Query: `db.product.find({$or:[{product_color:"indigo"},{product_price:492}]})`

10. **Delete the products which product price value is 28:**
    - MongoDB Query: `db.product.deleteMany({product_price:28})`

## Screenshots

Screenshots of each MongoDB query executed in MongoDB Compass are available in the PDF file.

