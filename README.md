# [React Node Material Kit PRO](https://appseed.us/product/react-node-js-material-kit-pro)

Material Dashboard PRO React is a Premium Material-UI Admin created using **create-react-app** with a fresh, new design inspired by Google's Material Design. The product comes with a simple JWT authentication flow: **login/register/logout** powered by a [Node JS API Server](https://github.com/app-generator/api-server-nodejs-pro) (PRO version). 

<br />

> Features

- Premium Material UI design - Designed by [Creative-Tim](https://bit.ly/3fKQZaL/)
- React, Redux, Redux-persist
- Authentication: JWT Login/Register/Logout
- [Node JS API server](https://github.com/app-generator/api-server-nodejs-pro) for a complete full-stack experience 

<br />

> Links

- [React Node Material Kit PRO](https://appseed.us/product/react-node-js-material-kit-pro) - product page
- [React Node Material Kit PRO](https://react-node-js-material-kit-pro.appseed-srv1.com) - LIVE Demo
- [Node JS API Server PRO](https://github.com/app-generator/api-server-nodejs-pro) (PRO version) - the backend server 
- Support via **Github** (issues tracker) and [Discord](https://appseed.us/support) - LIVE Assistance 

<br >

![React Node Material Kit PRO - Full-stack product built in React and Node JS by AppSeed and Creative-Tim.](https://user-images.githubusercontent.com/51070104/128535389-a09c68c2-02ec-4eb9-bad9-6bafcee85b10.png)

<br />

## How to use it

To use the product Node JS (>= 12.x) is required and GIT to clone/download the project from the public repository.

**Step #1** - Clone the project

```bash
$ git clone https://github.com/app-generator/priv-react-material-kit-pro.git
$ cd priv-react-material-kit-pro
```

<br >

**Step #2** - Install dependencies via NPM or yarn

```bash
$ npm i
// OR
$ yarn
```

<br />

**Step #3** - Start in development mode

```bash
$ npm run start 
// OR
$ yarn start
```

<br />

## Backend Integration

> The backend API server address is saved in `src/config/constant.js`.

```javascript
export const API_SERVER = "http://localhost:5000/api/";
```

<br />

> Frontend api has been created at `src/api/auth.js`.

```javascript
const axios = Axios.create({
    baseURL: `${baseURL}/api`,
    headers: { "Content-Type": "application/json" },
});
```    

<br />

> Register implementation:

- Frontend method with call to backend
- Form validation
- Error handling

<br />

> Login implementation:

- Frontend method with call to backend
- Form validation
- Error handling

<br />

> Logout implementation:

- Frontend method with call to backend

<br />

> User Context:

- The user account is now saved both to the React.Context wrapper and localStorage

<br />

> Protected routes:
 
- The user cannot access protected routes like /admin, /rtl without being logged in.
- Example of 3 different routes:

```javascript
    <ProtectedRoute path="/admin" component={AdminLayout} />
    <ProtectedRoute path="/rtl" component={RtlLayout} />
    <Route path="/auth" component={AuthLayout} />
```

<br />

> **API Server Descriptor** - POSTMAN Collection

The API Server definition is provided by the [Nodejs API Server](https://github.com/app-generator/api-server-nodejs)

- [API POSTMAN Collection](https://github.com/app-generator/api-server-nodejs/blob/master/media/api.postman_collection.json) - can be used to mock (simulate) the backend server or code a new one in your preferred framework. 

<br />

## Node JS API PRO

Express / Nodejs Starter with JWT authentication, and **SQLite** or **MongoDB** persistance - Provided by **AppSeed** [App Generator](https://appseed.us/app-generator).
Authentication Flow uses [json web tokens](https://jwt.io) via Passport library - `passport-jwt`.

> Features:

- Simple, intuitive codebase - can be extended with ease.  
- Typescript
- Data validation with Joy
- Branches:
    - **Master**: NodeJS / Express / SQLite / TypeORM
    - **Mongo**:  NodeJS / Express / MongoDB / Mongoose
- Auth: Passport / `passport-jwt` strategy 

<br />

> Requirements

- [Node.js](https://nodejs.org/) >= 10.x
- [SQLite](https://www.sqlite.org/index.html) - used by `master` branch
- [MongoDB](https://www.mongodb.com/) server - used by `mongo` branch

<br />

### How to use the code

**Clone the sources**

```bash
$ git clone https://github.com/app-generator/priv-api-server-nodejs-pro.git
$ cd priv-api-server-nodejs-pro
```

**Install dependencies** via NPM or Yarn

```bash
$ npm i
// OR
$ yarn
```

**Run the SQLite migration**

```
$ yarn typeorm migration:run
```

**Start the API server** - development mode

```bash
$ npm dev
// OR
$ yarn dev
```

**Production Build** - files generated in `build` directory

```bash
$ npm build
// OR
$ yarn build
```

**Start the API server** - for production (files served from `build/index.js`)

```bash
$ npm start
// OR
$ yarn start
```

The API server will start using the `PORT` specified in `.env` file (default 5000)

<br />

![Node JS API - Open-source API server built on top of Express Nodejs Framework.](https://user-images.githubusercontent.com/51070104/124934824-c210a700-e00d-11eb-9d01-e05bd8bfb608.png)

<br />

---
[React Node Material Kit PRO](https://appseed.us/product/react-node-js-material-kit-pro) - Provided by [Creative-Tim](https://bit.ly/3fKQZaL/) and **AppSeed [App Generator](https://appseed.us/app-generator)**. 
