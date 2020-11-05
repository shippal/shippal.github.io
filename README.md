## Welcome to Shippal !

Shippal is a set of website framework, include a e-commerce website, a backoffice website and a backend, build on top of React, Material-ui, nodejs and mongodb. You can use it as a template project to quickly build up your e-commerce web site with a backoffice.

You can use the [react-ecommerce](https://github.com/yocompute/react-ecommerce) to create your e-commerce front-end, with authentication product, shopping card, order, transaction and payment module ready to use, by default it will connect to shippal cloud as it's backend.

You can use the [react-backoffice](https://github.com/yocompute/react-backoffice) to create your e-commerce backoffice, by default it will connect to shippal cloud as it's backend.

Optionally, you can use the [node-ecommerce](https://github.com/yocompute/node-ecommerce) to create your e-commerce back-end, or you can choose to use shippal's cloud as your backend.

### Demo

Online Shop Demo
[react-ecommerce](https://www.yocompute.com)

Backoffice Demo
[react-backoffice](https://admin.yocompute.com)



### Install

### Install react-ecommerce
You can choose to install react-ecommerce without backend and database.

#### Install react-ecommerce without backend:
 step 1: Git clone the project
 step 2: CD to /react-ecommerce and run `npm install`
 step 3: Modify example.env to .env and change your jwt secret in .env, eg. JWT_SECRET=mysecret
 step 4: open your terminal and run `npm run`

You should be able to see the login page in your browser with http://localhost:3000

#### Install react-ecommerce with backend:
 step 1: Git clone the project
 step 2: CD to /react-ecommerce and run `npm install`
 step 3: Modify example.env to .env
 step 4: Change the value of MOCK to false in .env 
 step 5: Change values in .env to connect to your database, and other values if you need. For example you want change change your jwt secret you change the value of JWT_SECRET=x as JWT_SECRET=mysecret
 step 6: Start your node-ecommerce backend (see 'Install node-ecommerce' section ). If you have your node-ecommerce backend install and running up, you can skip this step.  
 step 7: open your terminal and run `npm run`
 
You should be able to see the login page in your browser with http://localhost:3000


### Install react-backoffice
You can choose to install react-backoffice without backend and database.

#### Install react-backoffice without backend:
 step 1: Git clone the project
 step 2: CD to /react-backoffice and run `npm install`
 step 3: Modify example.env to .env and change your jwt secret in .env, eg. JWT_SECRET=mysecret
 step 4: open your terminal and run `npm run`

You should be able to see the login page in your browser with http://localhost:3000

#### Install react-backoffice with backend:
 step 1: Git clone the project
 step 2: CD to /react-backoffice and run `npm install`
 step 3: Modify example.env to .env
 step 4: Change the value of MOCK to false in .env 
 step 5: Change values in .env to connect to your database, and other values if you need. For example you want change change your jwt secret you change the value of JWT_SECRET=x as JWT_SECRET=mysecret
 step 6: Start your node-commerce backend (see 'Install node-ecommerce' section ). If you have your node-ecommerce backend install and running up, you can skip this step.  
 step 7: open your terminal and run `npm run`
 
You should be able to see the login page in your browser with http://localhost:3000




### Test
`npm run test`

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
