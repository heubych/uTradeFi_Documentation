# Architecture

The architecture of uTradeFi is based on classic components of modern blockchain solutions.

## Front-end

The front-end is built with **React.js**. React is an open-source front-end JavaScript library for building solid user interface (UI) based on components. It is maintained by Meta and a community of developers and companies. React is one of the most popular technologies for building UI.

https://reactjs.org/

The front-end integrates all key components of the website:
* the investor pages to manage the composition of the synthetic trackers
* the pool performance underwriters pages to manage their positions
* the dashboards to show the state of the protocol at any time

## Back-end

The back-end is built with **Node.js**. Node.js is an open-source back-end JavaScript runtime environment and executes JavaScript code outside a web browser.

https://nodejs.org/en/

The back-end is used for API calls and interacts with the database.
* API to fetch quotes in real-time
* Caching of all required information for smooth browsing
* Bot surveillance of all active trades
* Database interactions: read and write

## Database

**MySQL** is used as central database for the protocol and stores all data used for reporting purpose. A lot of information is not required except for reporting and therefore don't need to be stored directly in the blockchain (for cost considerations). MySQL is a solid solution and interacts easily with the components describe above.

https://www.mysql.com/

## Blockchain

The smart contracts are Ethereum smart contracts built in Solidity. These smart contracts can be deployed on either Ethereum blockchain or Polygon. Depending on the release date of Ethereum 2.0 in 2022 the uTradeFi smart contracts will be deployed on one of these two blockchains. The current transaction costs on Ethereum are currently prohibitive for such a protocol (due to the number of transactions executed by the trading bots) and therefore the protocol will rely on a more cost efficient solution such as Ethereum 2.0 or Polygon.

## Dependencies

Main dependencies of the project for the UI:
* "react": "^17.0.2"
* "axios": "^0.24.0"
* "bootstrap": "^5.1.3"
* "ethers": "^5.5.2"
* "node-cache": "^5.1.2"
* "react-bootstrap": "^2.0.4"
* "react-dom": "^17.0.2"
* "react-icons": "^4.3.1"
* "react-router-dom": "^6.2.1"
* "react-scripts": "5.0.0"
* "react-slider": "^2.0.1"
* "recharts": "^2.1.10"

Main dependencies of the project for the backend:
* "cors": "^2.8.5"
* "dotenv": "^14.3.2"
* "express": "^4.17.2"
* "mysql": "^2.18.1",
* "node-fetch": "^3.1.1"
* "request": "^2.88.2"
