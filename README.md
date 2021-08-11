# React Node Material Kit PRO

**[Material Kit PRO React](https://appseed.us/product/react-node-js-material-kit-pro)** features over 1000 individual components, giving you the freedom of choosing and combining. The product comes with a simple JWT authentication flow: **login/register/logout** powered by a [Node JS API Server](https://github.com/app-generator/api-server-nodejs-pro) (PRO version). 

<br />

> Features

- Premium Material UI design - Designed by [Creative-Tim](https://bit.ly/3fKQZaL/)
- React, Redux, Redux-persist
- Authentication: JWT Login/Register/Logout
- Backend Server- [Node JS API Server PRO](https://github.com/app-generator/api-server-nodejs-pro)
    - SQLite / TypeORM / Joy / Docker
    - MongoDB / Mongoose / Joy Docker (separate branch, same project)

<br />

![React Node Material Kit PRO - Full-stack product built in React and Node JS by AppSeed and Creative-Tim.](https://user-images.githubusercontent.com/51070104/128535389-a09c68c2-02ec-4eb9-bad9-6bafcee85b10.png)

<br />

## How to use it

To use the product Node JS (>= 12.x) is required and GIT to clone/download the project from the public repository.

**Step #1** - Clone the project (private repository)

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

## API Server Node PRO

Express / Nodejs Starter with JWT authentication, and SQLite or MongoDB persistance. Authentication Flow uses json web tokens via Passport library - passport-jwt.

> Features

- Simple, intuitive codebase - can be extended with ease.  
- Typescript
- Data validation with Joy
- Branches:
    - **Master**: NodeJS / Express / SQLite / TypeORM
    - **Mongo**:  NodeJS / Express / MongoDB / Mongoose
- Auth: Passport / `passport-jwt` strategy 

<br />

### How to use the code

**Step #1** - Clone the project (private repository)

```bash
$ git clone https://github.com/app-generator/priv-api-server-nodejs.git
$ cd priv-api-server-nodejs
```

**Step #2** - Install dependencies via NPM or yarn

```bash
$ npm i
// OR
$ yarn
```

**Step #3** - Run the SQLite migration via TypeORM

```
$ yarn typeorm migration:run
```

**Step #4** - Start the API server (development mode)

```bash
$ npm dev
// OR
$ yarn dev
```

**Step #5** - Production Build (files generated in `build` directory)

```bash
$ npm build
// OR
$ yarn build
```

**Step #6** - Start the API server for production (files served from `build/index.js`)

```bash
$ npm start
// OR
$ yarn start
```

The API server will start using the `PORT` specified in `.env` file (default 5000). 

---
React Node Material Kit PRO - Provided by [Creative-Tim](https://bit.ly/3fKQZaL/) and **AppSeed [App Generator](https://appseed.us/app-generator)**. 
