# Description

A MERN React admin dashboard website that allows an admin user to see an overview of their shop.

# Tech Stack

## Front-end

- [React](https://react.dev/)
- [React Router](https://reactrouter.com/en/v6.3.0/getting-started/installation)
- [Redux Toolkit](https://redux-toolkit.js.org/introduction/getting-started)
- [Redux Toolkit Query](https://redux-toolkit.js.org/rtk-query/overview)
- [Material UI](https://mui.com/material-ui/getting-started/installation/)
- [Nivo](https://nivo.rocks/)

## Backend

- [MongoDB](https://www.mongodb.com/)
- [MongoDB Aggregate](https://www.mongodb.com/docs/manual/reference/operator/aggregation-pipeline/)

# Usage

1. Clone this repository.
   `git clone https://github.com/rebkang/admin-app.git`

2. Create a [MongoDB](https://www.mongodb.com/) account and connect your app to it.

3. Navigate to the `server` directory and create a `.env` file. Add the following:

```
MONGO_URL = <url-to-your-mongo-db>
PORT=5001
```

4. Uncomment the part in `server/index.js` that talks about importing data. After the first run of the server, make sure to re-comment this.

```
// AffiliateStat.insertMany(dataAffiliateStat);
// OverallStat.insertMany(dataOverallStat);
// Product.insertMany(dataProduct);
// ProductStat.insertMany(dataProductStat);
// Transaction.insertMany(dataTransaction);
// User.insertMany(dataUser);
```

5. Install the dependencies in the `server` file.
   `npm i`

6. Navigate to the `client` directory and create a `.env` file. Add the following:
   `REACT_APP_BASE_URL=http://localhost:5001`

7. Install the dependencies in the `client` file.
   `npm i`

8. Open up two terminals and run these commands:

```
cd server
npm run dev
```

```
cd client
npm run start
```
