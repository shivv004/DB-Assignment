# DB-Assignment Solution

## 1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.
### The relationship between the Product and Product_Category is one-to-many relationship.
### It means that each product belongs to only one category, but each category can have multiple products associated with it. This is represented by the line between Product_Category and Product.
### The symbol on the line at the "Product" end indicating "many" and the symbol at the "Product_Category" end indicating "one".

## 2. How could you ensure that each product in the "Product" table has a valid category assigned to it?
### To ensure that each product in the Product table has a valid category assigned to it, we can use a referential constraint. For example in sql we can create a foreign key constraint in "Product" table with references to the primary key of "Product_Category" table. This will ensure that every value in the foreign key column(category_id) of the "Product" table must exist as a primary key(id) value in the "Product_Category" table.
