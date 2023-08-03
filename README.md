# Contact_Manager_Backend_Project
Contact Manager Web App Backend
The Contact Manager Web App Backend is a Node.js and Express.js based web application that serves as the server-side for a contact manager web application. It utilizes MongoDB as the database for storing user information and contact records. The backend provides various endpoints to handle user authentication and perform CRUD operations on contacts.

__Features:__

__User Authentication:__
The backend supports user registration and login functionality. Users can register with a unique username and password, and their credentials will be securely stored in the database. For subsequent interactions with the API, users need to log in using their registered credentials to gain access to their contacts.

__JSON Web Token (JWT) Authentication:__
To ensure secure user sessions, the backend uses JSON Web Tokens (JWT) for authentication. After successful login, the server generates a JWT token, which the client must include in the headers of authenticated requests. This token allows the backend to verify the user's identity and permissions for each operation.

__Contact Management:__
Authenticated users can perform CRUD (Create, Read, Update, Delete) operations on their contacts. The backend provides endpoints to create new contacts, retrieve a list of all contacts, update existing contacts, and delete unwanted contacts.

__MongoDB Database:__
The application uses MongoDB as the database to store user information, such as usernames and hashed passwords, as well as contact records. MongoDB's flexibility allows easy management and retrieval of data, making it a suitable choice for this web application.

__Endpoints:__
The backend provides the following endpoints:

POST /api/users/register: Register a new user with a unique username and password.

POST /api/users/login: Log in an existing user and receive a JWT token for further authentication.

GET /api/users/current: Retrive the current user Contacts

GET /api/contacts: Retrieve all contacts for the authenticated user.

GET /api/contacts/:id: Retrieve a certain contact for the authenticated user.

POST /api/contacts: Create a new contact for the authenticated user.

PUT /api/contacts/:id: Update an existing contact for the authenticated user.

DELETE /api/contacts/:id: Delete an existing contact for the authenticated user.
