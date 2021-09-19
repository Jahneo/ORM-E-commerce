# 13 Object Relational Mapping (ORM): E-commerce Back End Starter Code
# Task
Challenge is to build the back end for an e-commerce site. You’ll take a working Express.js API and configure it to use Sequelize to interact with a MySQL database.
Because this application won’t be deployed, you’ll also need to create a walkthrough video that demonstrates its functionality and all of the following acceptance criteria being met. You’ll need to submit a link to the video and add it to the README of your project.
# User Story
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies
# Acceptance Criteria
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia Core for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete data in my database
# Mock-Up
The first animation shows GET routes to return all categories, all products, and all tags being tested in Insomnia Core:
![Demo1](.Develop/assets/images/demo-01.gif)
The second animation shows GET routes to return a single category, a single product, and a single tag being tested in Insomnia Core:
![Demo2](.Develop/assets/images/demo-02.gif)
The final animation shows the POST, PUT, and DELETE routes for categories being tested in Insomnia Core:
![Demo3](.Develop/assets/images/demo-03.gif)
# Packages
MySQL2 and Sequelize packages to connect your Express.js API to a MySQL database and the dotenv package(store sensitive data)
# Database Models
Categories
    Product
        Tag
            Product Tag
# Associations
    * Product belongs to Category, as a category can have multiple products but a product can only belong to one category.
    * Category has many Product models
    * Product belongs to many Tag models. Using the ProductTag through model, allow products to have multiple tags and tags to have many products.
    * Tag belongs to many Product models.

   
