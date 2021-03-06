demandware-angularjs-seed
=========================

An AngularJS mini-site for show up data from Demandware

- A Demandware mini-site with AngularJS (Inspired by http://yeoman.io)
- A showcase ecommerce site with frontend requirement
- No need server side scripting (NodeJS or Grunt only for deploy)

Features:

- [x] Twitter Bootstrap 3.x (Inspired by http://www.bootstrapzero.com/bootstrap-template/mpurpose)
- [x] Responsive
- [x] Navigation menu
- [x] Show root categories 
- [x] Show category products
- [x] Show standard product detail page
- [ ] Show product page with complex data (variation, set, bundle)
- [ ] Shopping cart
- [ ] Checkout

Screenshots:

Category page screenshot:
![alt text](https://raw.githubusercontent.com/nhduy1985/demandware-angularjs-seed/develop/screenshots/ss_category_1.png "Category Page")

Product page screenshot:
![alt text](https://raw.githubusercontent.com/nhduy1985/demandware-angularjs-seed/develop/screenshots/ss_product_1.png "Product Page")

Requirements
============

*Only for developement and deployment*

1. NodeJS http://nodejs.org
2. Grunt http://gruntjs.com


Installation
============

1. Download the repo

2. Install ``grunt``

 ```
 npm -g grunt-cli
 ```
 
3. Install packages

 ```
 npm install
 bower install
 ```
4. Configuration
 ```
 //create config file from template
 cp app\scripts\config.js.dist app\scripts\config.js
 
 //configure the config file
 vm app\scripts\config.js
 ```
 
 *Notes:*
 - OCAPI configuration see more at https://info.demandware.com/DOC1/topic/help/OCAPI/13.6/usage/APIUsage.html
 - Don't forget to add runing server to 'allowed_origins' in Business Admin

Running
=======

1. Development
 ```
 grunt server
 ```
 
2. Deployment
 ```
 //Step 1: build the 'dist'
 grunt build
 
 //Step 2: upload the 'dist' to the server
 ```
 