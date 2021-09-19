# ecommerce-back-end

# Description
This repo represent a back-end infratucture to support an ecommerce site via expressJS which will use Sequelize as on ORM to interact with a MySQL database. 

# Table of Contents 
* [Installation](#installation)
* [Usage](#usage)
* [Tests](#test)
* [Contributing](#​contributors)
* [Contact Me](#contact-me)
* [License](#license)


## Installation
````
 1. To create the database for the first time
    a. cd to the project root directory 
    b. mysql -u <username> -p
    c. Enter Password
    d. Run source b/schema.sql
2. Run npm run start
3. To initially load the database, npm run seed
````

## Usage
Use Insomnia for the following routes:
### Category
1. To list all Categories<br /> 
    GET http://localhost:3001/api/categories 

2. To find one category <br /> 
    GET http://localhost:3001/api/categories/:id

3. To create a new cateogry <br /> 
    POST http://localhost:3001/api/categories/ <br /> 
    {
	    "category_name" : "value"
    }   
4. To update a category <br /> 
    PUT http://localhost:3001/api/categories/:id <br /> 
    {
	    "category_name" : "value"
    } 
5. To delete a cateogry <br /> 
    DELETE http://localhost:3001/api/categories/:id

### Tags
1. To list all tags <br /> 
    GET http://localhost:3001/api/tags

2. To find one tag <br /> 
    GET http://localhost:3001/api/tags/:id

3. To create a new tag <br /> 
    POST http://localhost:3001/api/tags/ <br /> 
    {
	    "tag_name" : "value"
    }   
4. To update a tag <br /> 
    PUT http://localhost:3001/api/tags/:id <br /> 
    {
	    "tag_name" : "value"
    } 
5. To delete a tag <br /> 
    DELETE http://localhost:3001/api/tags/:id

### Products
1. To list all products <br /> 
    GET http://localhost:3001/api/products

2. To find one product <br /> 
    GET http://localhost:3001/api/products/:id

3. To create a new product <br /> 
    POST http://localhost:3001/api/products/ <br /> 
   {
      "product_name": "Basketball",
      "price": 200.00,
      "stock": 3,
      "tagIds": [1, 2, 3, 4],
	 "category_id" : 5
 }  
4. To update a product <br /> 
    PUT http://localhost:3001/api/products/:id <br /> 
 {
      "product_name": "Basketball",
      "price": 200.00,
      "stock": 3,
      "tagIds": [1, 2, 3, 4],
	  "category_id" : 5
 }
5. To delete a products <br /> 
    DELETE http://localhost:3001/api/products/:id

## ​Walkthough Videos
Viewo Walkthrough (Setup): https://drive.google.com/file/d/1jIhz6YKpInDHb0-DwsBMhbSkFH7qZTuG/view?usp=sharing
Video Walkthrough (Category): https://drive.google.com/file/d/1WELbIeXSHcoCjP2xnLVGsDGu-VVDAXa-/view?usp=sharing
Video Walkthrough (Products): https://drive.google.com/file/d/1Pj7_H-tzbqSjYwWv2PR1O99CaT4LWojj/view?usp=sharing
Video Walkthrough (Tags): https://drive.google.com/file/d/1ExlYJNwD3aElySSO9UumRMdlRPPeDshl/view?usp=sharing


## ​Contributors
* Starter Code Can Be found at: <https://github.com/coding-boot-camp/fantastic-umbrella>


## Contact Me
For Issues please create a github issue for the repository

 
## License
This  project is currently unlicensed 

