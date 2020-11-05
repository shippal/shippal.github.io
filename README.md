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



### Install react-ecommerce
You can choose to install react-ecommerce without backend and database or choose [node-ecommerce](https://github.com/yocompute/node-ecommerce) as your backend..

#### Install react-ecommerce without backend:
1. Git clone the project from [react-ecommerce](https://github.com/yocompute/react-ecommerce)
2. CD to /react-ecommerce and run `npm install`
3. Modify example.env to .env and change your jwt secret in .env, eg. JWT_SECRET=mysecret
4. open your terminal and run `npm run`

You should be able to see the login page in your browser with http://localhost:3000

#### Install react-ecommerce with node-ecommerce as backend:
1. Git clone the project [react-ecommerce](https://github.com/yocompute/react-ecommerce)
2. CD to /react-ecommerce and run `npm install`
3. Modify example.env to .env
4. Change the value of MOCK to false in .env 
5. Change values in .env as following (assume your backend run at port 8006): 
```
REACT_APP_LOCAL_DATA=false
REACT_APP_API_URL = http://localhost:8006/api
```
6. Start your node-ecommerce backend (see 'Install node-ecommerce' section ). If you have your node-ecommerce backend install and running up, you can skip this step.  
7. open your terminal and run `npm run`
 
You should be able to see the login page in your browser with http://localhost:3000


### Install react-backoffice
You can choose to install react-backoffice without backend and database.

#### Install react-backoffice without backend:
1. Git clone the project [react-backoffice](https://github.com/yocompute/react-backoffice)
2. CD to /react-backoffice and run `npm install`
3. Modify example.env to .env and change your jwt secret in .env, eg. JWT_SECRET=mysecret
4. open your terminal and run `npm run`

You should be able to see the login page in your browser with http://localhost:3000

#### Install react-backoffice with node-ecommerce as backend:
1. Git clone the project [react-backoffice](https://github.com/yocompute/react-backoffice)
2. CD to /react-backoffice and run `npm install`
3. Modify example.env to .env
4. Change the values in .env as following (assume your backend run at port 8006): 
```
REACT_APP_API_URL = http://localhost:8006/api
REACT_APP_MODE = remote
```
6. Start your node-commerce backend (see 'Install node-ecommerce' section ). If you have your node-ecommerce backend install and running up, you can skip this step.  
7. open your terminal and run `npm run`

You should be able to see the login page in your browser with http://localhost:3000


### Install node-ecommerce as backend

Though node-ecommerce only supports mongodb as database for now, we will support any other popular database like mysql, postgrad ...

You need firstly create your mongodb,  then configure your mongodb authentication (config authentication is optional, but highly recommand when you host in production ), we skip the mongodb install here, you can refer [mongodb community server page](https://docs.mongodb.com/manual/administration/install-community/) for installation.

For configure mongodb to use authentication, you can refer [start the mongod using a configuration file, add the security.authorization configuration file setting] (https://docs.mongodb.com/manual/tutorial/enable-authentication/) 

For mongodb credential, you can refer [add mongodb user and credential](https://docs.mongodb.com/manual/tutorial/create-users/)

1. Git clone the project from [node-ecommerce](https://github.com/yocompute/node-ecommerce)
2. CD to /react-backoffice and run `npm install`
3. Modify example.env to .env
4. Change values in .env to connect to your database (replace the content in < >)

If you don't have database authentication, you can set DB_AUTH=false as following:
```
MOCK=false
DB_AUTH=false
DB_NAME=<my database name>
```

If you have database authentication, you need to set DB_AUTH=true and set your credential as following:
```
MOCK=false
DB_AUTH=true
DB_NAME=<my database name>
DB_USERNAME=<my database username>
DB_PASSWORD=<my database password>
DB_AUTH_SOURCE=<my authentication database name>
```

5. Change other values if you need. For example you want change change your jwt secret you change the value of JWT_SECRET=x as JWT_SECRET=mysecret
6. open your terminal and run `npm run`

You should be able to see 'API listening at http://localhost:8006' in your terminal


### Test
Open a terminal, CD to any of above 3 project folder and run `npm run test`

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
