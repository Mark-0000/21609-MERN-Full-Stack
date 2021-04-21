# 21609-MERN-Full-Stack

Continuous Assessment 2 for Back-End Web Development

## How to run
npm init - this will install all the dependencies required \
npm run dev - the application will run both the client server and api server using concurrently

### api server
express - server\
mongodb - database\
body-parser - json parser for response and requests\

the server uses port from .env file or 8080 and body-parser as a middleware\

the api server responses to 4 routes\
1. /GET/api/users - returns all the data from the database\
2. /GET/api/users/:id - return a specific data using ID as a parameter\
3. /DELETE/api/users - delete a specific data from the database using ID as the body\
4. /POST/api/users - inserts data to the database\
5. /PUT/api/users - update data from the database\

### client server
the client server was built in react which is a single page application \
the client has 6 components/pages which can be navigated using react-router-dom

the client has 6 components\
1. index - this is the driver that renders all information to the index.html file\
2. App - the main/parent components which renders the page based on the route\
3. UserList - child component of App and parent component of User which renders all the User data \
4. User -  child component of UserList which renders data of a specific object in a card\
5. CreateUser -  child component of App which renders the form and handles the POST request to the server\
6. EditUser -  child component of App which renders the data of a specific object in a form to be edited and handles the PUT request to the server


