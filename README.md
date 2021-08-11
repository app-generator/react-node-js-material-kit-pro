# React Material Kit PRO

Material Dashboard PRO React is a Premium Material-UI Admin created using **create-react-app** with a fresh, new design inspired by Google's Material Design. The product comes with a simple JWT authentication flow: **login/register/logout** powered by a [Node JS API Server](https://github.com/app-generator/api-server-nodejs-pro) (PRO version). 

<br />

> Features

- Premium Material UI design - Designed by [Creative-Tim](https://bit.ly/3fKQZaL/)
- React, Redux, Redux-persist
- Authentication: JWT Login/Register/Logout
- For a complete full-stack experience, this UI can be used with:
  - [Django API Server](https://docs.appseed.us/boilerplate-code/api-server/django) - open-source product
  - [Flask API Server](https://docs.appseed.us/boilerplate-code/api-server/flask) - open-source product
  - [Node JS API Server](https://docs.appseed.us/boilerplate-code/api-server/node-js) - open-source product / Typescript / SQLite / TypeORM / Joy for validation
  - [Node JS API Server PRO](https://github.com/app-generator/api-server-nodejs-pro) - **commercial product**
      - SQLite / TypeORM / Joy / Docker
      - MongoDB / Mongoose / Joy Docker (separate branch, same project)

<br />

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

> **API Descriptor** 

The product uses implements a **Unified API definition** exposed by all API servers crafted by AppSeed. For more information, please access the official documentation:

- All [API Servers](https://docs.appseed.us/boilerplate-code/api-server) - the full index
- [Unified API Definition](https://docs.appseed.us/boilerplate-code/api-server/api-unified-definition) - methods implemented accross all servers


<br />

---
React Material Kit PRO - Provided by [Creative-Tim](https://bit.ly/3fKQZaL/) and **AppSeed [App Generator](https://appseed.us/app-generator)**. 
