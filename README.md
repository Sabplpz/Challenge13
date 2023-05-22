# E-Commercer Back End - Challenge 13

## Description

This project is the back end side of an E-Commercer website, which allows you to get the information about categories, products and tags you need, eithe rit being for all or just one. You can also add new categories, products and tags, as well as update or delete them. This will her this business maintain orginazation as well as their site upto date with their business. I learnt a lot about routes on this challenge!

## Table of Contents

If your README is long, add a table of contents to make it easy for users to find what they need.

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)
- [Links](#links)

### Installation

As of right now, this is not a deployed site, so you will need to download all documents as well as the app Insomnia to try this out. Don't forget to add your MySQL credentials!

### Usage

To use this back end app, you will need to start the server and go into the Insomnia app. Once there, you can start using the next lines to try all our routes:

GET: http://localhost:3001/api/categories
GET: http://localhost:3001/api/categories/1 (Try with any ID)
GET: http://localhost:3001/api/products
GET: http://localhost:3001/api/products/1 (Try with any ID)
GET: http://localhost:3001/api/tags
GET: http://localhost:3001/api/tags/1 (Try with any ID)

![alt text](assets/try1.gif)

POST: http://localhost:3001/api/categories (Create new category)
JSON: {"category_name": "Example"}
POST: http://localhost:3001/api/tags (Create new tag)
JSON: {"tag_name": "Example"}
POST: http://localhost:3001/api/products (Create new product)
JSON: {
      "product_name": "Basketball",
      "price": 200.00,
      "stock": 3,
      "tagIds": [1, 2, 3, 4]
      }

![alt text](assets/try2.gif)

To delete:
DELETE: http://localhost:3001/api/categories/1
DELETE: http://localhost:3001/api/products/1
DELETE: http://localhost:3001/api/tags/1

To update:
PUT: http://localhost:3001/api/categories/1
JSON: {"category_name": "Example"}
PUT: http://localhost:3001/api/products/1
JSON: {
      "product_name": "Basketball",
      "price": 200.00,
      "stock": 3,
      "tagIds": [1, 2, 3, 4]
      }
PUT: http://localhost:3001/api/tags/1
JSON: {"tag_name": "Example"}

![alt text](assets/try3.gif)

### Credits

As always, thanks to my amazing tutor, Mansi! And of course thanks to me :)

### License

MIT License

### Links

Repo: https://github.com/Sabplpz/E-commerceBackEnd
Walkthrough video: https://drive.google.com/file/d/1-VxDgyWP3qnRIy_HiyhL05HSeITEModw/view
