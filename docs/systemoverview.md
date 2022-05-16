# Architecture

The basic architecture of uTradeFi is based on classic components of modern blockchain solutions.

Content to be written!

## Front-end

The front-end is built with **React.js**. React is an open-source front-end JavaScript library for building solid user interface (UI) based on components. It is maintained by Meta and a community of developers and companies. React is one of the most popular technologies for building UI.

https://reactjs.org/

The front-end integrate all key components of the website:
* the investors pages to manage their synthetic trackers
* the pool performance underwriters pages to manage their position into the protocol
* the dashboards to show the state of the protocol at any time

## Back-end

The back-end is the server part of the infrastructure. The back-end is built with **Node.js**. Node.js is an open-source back-end JavaScript runtime environment and executes JavaScript code outside a web browser. The back-end is used for API calls and interacts with the database.

https://nodejs.org/en/

## Database

**MySQL** is used as central database for the protocol and stores all data used for reporting purpose. A lot of information is not required except for dashboarding purpose and therefore don't need to be stored in the blockchain (for cost considerations). MySQL is a solid solution and interacts easily with the components describe above.

https://www.mysql.com/

## Blockchain

Ethereum! Polygon!
