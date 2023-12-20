# Eas-E-commerce

## Description
This program is a backend api handler and database storage tool for an e-commerce business. The motivation for building this project was to deploy the sequelize ORM model to the tables for a database. It allows a business to store product information that can be manipulated through all of the CRUD calls via RESTFUL api's. I learned out to effectively instantiate a database with mysql, use a set of ORM models to create the tables and relationship structure, then asynchronously call then pass all the CRUD calls to successfully manage the db. 


## Installation
Before cloning this repo a mysql data base will need to be set up and then connected to the program.  The mysql database schema can be found in the `db` directory and can be run to set up the `ecommerce_db`. After setting up the mysql table you can login to the data base by creating a .env file and entering your db credentials into the following fields:

`
DB_NAME=''
DB_USER=''
DB_PW=''
`

DB_Name will be "ecommerce_db" and the other two  will be your personal mysql login information.

After mysql database is set up clone the repo, run `npm install` in the main directory and start the server with `npm start`.  

After running npm start the ORM models will automatically be called and sync to form 4 tables in the ecommerce_db:

1. category
2. product
3. tag 
4. product tag (junction table)

You can then use your choice of tool such as Insomnia or POSTman to make api calls.

## Usage

A demonstration of the endpoints for the Category, Tag, and Product API calls can be viewed here: [Walkthrough](https://drive.google.com/file/d/1V4LI9P7S_3YtOkADM4AiHB9q4L5k57CN/view?usp=drive_link)


Each of the three main tables (category, tag, and product) can be called using the following endpoints:

1. GET (Read) all 
2. GET (Read) by id
3. POST (Create) 
4. PUT (Update) by id
5. DELETE (Delete) by id

The relationships are predefined in the ORM. 

## Credits

Git Bootcamp Content - ORM Activities. (n.d.). Retrieved from https://git.bootcampcontent.com/University-of-Texas-at-Austin/UTA-VIRT-FSF-PT-09-2023-U-LOLC/-/tree/main/13-ORM?ref_type=heads

Sequelize Documentation. (n.d.). Retrieved from https://sequelize.org/docs/v6/getting-started/

## Questions
GitHub Repo: https://github.com/Spencox/Eas-E-commerce   
Email: spencox@gmail.com

