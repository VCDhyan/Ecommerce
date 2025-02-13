E-Commerce Application: Backend Web Development Project
Milestone 1: Project Overview
Brief Overview: This project involves developing a fully functional e-commerce platform utilizing the MERN stack — MongoDB, Express, React, and Node.js. The application will be built using React's Create React App (CRA) for the front-end, MongoDB as the database solution, and Node.js with Express to handle the back-end server operations.

The project will be split into two main areas: Frontend (client-side) and Backend (server-side) development.

Frontend: We will be creating various pages for user interaction, including:

Login Page
Sign Up Page
Forgot Password Page
Home Page
Product Display Page
Cart Page
Address Page
Payment Page
Order Confirmation Page
Order History Page
Help Page
Error Page
Detailed Product Pages
Backend: The server will interact with MongoDB, a NoSQL database, to handle data management. We will be using the Mongoose library to interact with the database and define schemas for data consistency. To manage communication between the front-end and the back-end, we will implement APIs that allow for CRUD operations (Create, Read, Update, Delete) using HTTP methods like POST, GET, PUT, PATCH, and DELETE.

We’ll integrate bcrypt for password hashing to ensure user data security, and the entire project will follow best practices for backend structure, focusing on scalability and maintainability.

Milestone 2: Frontend Development (Login Page)
For this milestone, we successfully created the Login Page using React's Create React App (CRA). To improve the user interface and design, we will be updating the layout with Tailwind CSS for styling and incorporate React-Icons for intuitive icons. Tailwind CSS will help us streamline the design process with its utility-first classes, making the UI responsive and visually appealing.

The Login Page will include fields for the user's email and password, and will handle form validation, state management, and error handling for incorrect login attempts. React Icons will be utilized for visual appeal and ease of use, enhancing the overall experience.

Milestone 3: Backend Structure and Initial Setup
At this stage, we’ve laid the foundation for the backend by setting up the directory structure for the project. The backend is structured as follows:

src/ Directory: Contains all source code files for the server.
config/: Stores environment configuration files like .env for MongoDB URL and the server port.
controllers/: Defines functions to handle incoming requests for various routes.
database/: Contains the MongoDB connection logic in db.js.
middleware/: Houses custom middleware functions such as error.js for centralized error handling.
model/: Contains Mongoose models for the database schema.
routers/: Defines route handlers for different API endpoints.
utils/: Stores utility functions, including the ErrorHandler.js to manage application-level errors.
In the index.js file, we imported Express, initialized the app, and set up basic routing and server listening. We can now handle HTTP requests through app.get and set the server to listen for incoming requests on the specified port.

Milestone 4: Backend Structure and Initial Setup
creating user model, user controller and Multer support

**Milestone 6
: Backend Structure and Initial Setup** Password Encryption and User Data Storage

Password Hashing:

Implement bcrypt to hash the user's password during the signup process. Ensure that the hashed password is stored in the database instead of the plaintext version to enhance security. User Data Storage:

Save all relevant user information (e.g., name, email, etc.) in the database. Maintain the integrity and confidentiality of the password by ensuring it remains encrypted throughout the process.

**Milestone 7
Create Login Endpoint:

Accept user credentials (email/username and password). Retrieve the corresponding user from the database. Validate Password:

Use bcrypt to hash the entered password. Compare it with the stored hashed password for authentication.

**Milstone 8
In this milestone we created two components called Home.jsx and productcard.jsx. product card.jsx is the template used in home.jsx to map out all the products and display them. We also added routes to the home.jsx to display it when the page loads. Based on the number of products the products are mapped and displayed.

Product Management System – Milestone 12

In this milestone, we’ll create an API endpoint to retrieve all products filtered by a user’s email and send that data to the frontend.

We will also build a function in the frontend to fetch this filtered data and display it dynamically using the ProductCard component.

Why This Milestone is Important

Understanding Data Filtering: Learn how to filter data based on specific criteria (e.g., user email) and send only relevant data to the frontend.

Dynamic Data Handling: Enhance your ability to retrieve and display data dynamically using React components.

Practical Experience with Filtering: This skill is essential for real-world applications, like showing only products created by a specific user.

Steps for Milestone 12

Backend: Writing the Endpoint to Retrieve Filtered Product Data

We’ll create a GET endpoint that fetches all products associated with a specific user’s email from the database.

Frontend: Fetching Filtered Data from the Backend

On the frontend, we’ll create a function to call the new API endpoint and fetch products for a specific user email.

Creating the Product Card Component

This component will display each product’s details, just like in previous milestones.

How This Works

Backend: The GET endpoint filters the products in MongoDB by the userEmail field and returns the results.

Frontend: The fetchUserProducts function fetches the filtered data based on the provided email.

Dynamic Rendering: The data is passed to the ProductCard component, which renders a card for each product that belongs to the specified user.
In this milestone, we’ll build an API endpoint to fetch all product data from the database and display it dynamically on the frontend using a reusable product card component.

Why This Milestone is Important

Learn to Send and Receive Data: Understand how to connect the frontend and backend to retrieve data.

Dynamic Rendering: Display data dynamically by passing it to components, improving scalability and efficiency.

Reusable Components: Use a single component to display multiple products without writing repetitive code.

How it works :

Backend: The GET endpoint fetches all products from the MongoDB database.

Frontend: The fetchProducts function calls the API to get the product data.
Product Management System

This project focuses on building a simple product management feature using Node.js, Express, MongoDB, and Mongoose.

You’ll create a Product Schema, set up an API endpoint to save product data, and learn how to ensure data integrity through validation.

Why Product Schema and Validation Matter

Product Schema: Defines how product data is structured in the database. It ensures consistency and makes it easier to manage the data.

Validation: Protects your application by ensuring only valid data is stored in the database. This helps prevent errors and maintains data integrity.

Features

Create a product with fields like name, description, price, and image URL.

Validate input data to ensure required fields are filled with the correct data types.

Save the validated product data to MongoDB.
