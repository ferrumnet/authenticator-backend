# Ferrum Network Authenticator Backend
======================

Overview
--------

This is the backend part of the Ferrum Network project, which validates user addresses via Web3. Users sign a message including a nonce with their Ethereum private key, and the backend verifies the signed message to ensure ownership of the corresponding Ethereum address.

Features
--------

1.  Address Verification: Using Web3, the backend verifies Ethereum addresses by checking signed messages from users.
2.  Express.js Server: The backend runs on an Express.js server, providing a fast, unopinionated, and minimalist web framework for Node.js.
3.  CORS Enabled: The server is CORS enabled, allowing it to receive requests from different domains.
4.  Environment Variables: With the help of dotenv, environment variables from your .env file are loaded.

Setup & Run
-----------

Before running the server, make sure to have Node.js and npm/yarn installed on your machine.

### Installation

1.  Clone the repository:

```sh
git clone <repo-link>
```

2.  Navigate into the repository:

```sh
cd ferrum-network-backend
```

3.  Install the dependencies:

```sh
npm install
```

or

```sh
yarn install
```

### Configuration

Create a `.env` file in the root directory and define your environment variables:

```sh
PORT=<port>
```

Replace `<port>` with the port you want the server to listen on. The default port is `8081` if not specified.

### Run the Server

To run the server, use the command:

```sh
npm start
```

or

```sh
yarn start
```

This will start the server, and it will start listening on the port you defined.

API Endpoints
-------------

The server currently has the following endpoints:

-   GET `/` - Test endpoint that responds with a greeting.
-   POST `/verify` - Verifies a signed message and checks the ownership of an Ethereum address.

Contribution
------------

Feel free to contribute to this project by creating issues or pull requests. We welcome any feedback or suggestions.

License
-------

This project is licensed under the terms of the MIT license. For more details, see the LICENSE file.