Thursday
Thursday


Thursday
 Thursday main
73bb6a53972cb839144a18ce3ba457ceb03ffb30
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

## Milestone 2: Frontend Development (Login Page)
For this milestone, we successfully created the Login Page using React's Create React App (CRA). To improve the user interface and design, we will be updating the layout with Tailwind CSS for styling and incorporate React-Icons for intuitive icons. Tailwind CSS will help us streamline the design process with its utility-first classes, making the UI responsive and visually appealing.

The Login Page will include fields for the user's email and password, and will handle form validation, state management, and error handling for incorrect login attempts. React Icons will be utilized for visual appeal and ease of use, enhancing the overall experience.

## Milestone 3: Backend Structure and Initial Setup
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

## Milestone 4: Backend Structure and Initial Setup
creating user model, user controller and Multer support

Milestone 6
: Backend Structure and Initial Setup** Password Encryption and User Data Storage

Password Hashing:

Implement bcrypt to hash the user's password during the signup process. Ensure that the hashed password is stored in the database instead of the plaintext version to enhance security. User Data Storage:

Save all relevant user information (e.g., name, email, etc.) in the database. Maintain the integrity and confidentiality of the password by ensuring it remains encrypted throughout the process.

Milestone 7
Create Login Endpoint:

Accept user credentials (email/username and password). Retrieve the corresponding user from the database. Validate Password:

Use bcrypt to hash the entered password. Compare it with the stored hashed password for authentication.

Milestone 8
In this milestone we created two components called Home.jsx and productcard.jsx. product card.jsx is the template used in home.jsx to map out all the products and display them. We also added routes to the home.jsx to display it when the page loads. Based on the number of products the products are mapped and displayed.

Milestone 9 - Product Form Creation
Overview

In this milestone, I created a product form designed to collect all necessary details for new products. This form is essential for inputting data that will be stored in the MongoDB database and displayed on the product page, which was made in the previous milestone.

Steps Taken

Form Development: I designed and implemented a user-friendly form that allows for the input of multiple products, images along with other relevant product details such as name price description catagory tags... etc.

For this milestone I mostly worked on the frontend of the project. I created a new file named as the productform.jsx.

Milestone 10
In this milestone I created a schema for products. I made this using a new js file in the Model folder named Productmodel.js. In this I used mongoose to make the schema. I also created a new file called Products.js when I have all the program for initiating a post request that will store all the data in the database. I also used the middleware Multer to process and use the image files that would be uploaded of the product.I have made the neccessary changes to the middleware folder and Index.js to work as intended.

Milestone 11 and 12
In this milestone we bridged the gap between the frontend and the backend of the productform by connecting it to mongoDB. In the first milestone we made changes to products.js to use the get router to find the data in mongo db and pass it forward to home.jsx where it would then be displayed to show the products that are present on the database. In milestone 2 we were supposed to use nodemailer but it was not done as our mentor said it was unneccesary. Then we made changes to the post router to make the form functional and make it upload new products to the database.

Milestone 13
In this milestone we made the endpoint for updation. We use the put request to carry it out. In the frontedn we added the delete and edit buttons for editing and deleteing. Also since it should only be visible to the seller we made a whole new productcard.jsx for sellers.

Milestone 14
added an functionality to delete button to the product data and write and backend endpoint to delete the product with the use of ID. Also fixed some of the other bugs I faced which were causing unexpected behaviours and made the routing much more clear.

Milestone 15
In this milestone I created a new navbar that renders on all the pages. I added Navlinks for Home, productform, login and signup. I first made a new jsx file called navbar and then created the whole navbar. I also styled it using Tailwind css. I also had other issues that I fixed in home.jsx and styled productform jsx as it had no styling before.

Milestone 16
Created singleproduct.jsx. The pages is made to show details about the product. I also routed it and made other minor changes.

Milestone 17 & 18
In these two Milestones we first added the cart details to the schema. Then we also created a post request for sending the details and storing them on the database. We also created an endpoint to receive request from cart page.

Milestone 19
create cart frontend page and display the products For each product add an option to increase and decrease quantity using + and - buttons. Create an Backend endpoint for increase and decrease quantity

Milestone 23
Create an placeorder button inside cart page and navigate to select address page when clicked. Create and select address page that will display all the available address and have an option to select one address. Write an backend endpoint that will send all the addresses of the user.

Milestone 27
You need to create an my-orders page You will send an get request to my-orders endpoint that we created in previous milestone. We will send user mail in to endpoint to get all the user orders Display all the user orders We will add my-orders page in navbar for better navigation.

Milestone 21
create address form frontend page Create an state that will store input address when we click on add address in profile it should navigate to this form page.

E-Commerce-_FollowAlong
Features
1. Authentication Page
User Login and Signup functionality.
Password security with hashing.
Token-based authentication for session management.
2. Product Page
Displays a list of available products.
Search and filter functionality for efficient product browsing.
3. Order Page
View all past orders with relevant details (product name, price, date).
Track the status of current orders.
4. Payment Gateway
Multiple payment methods (credit/debit card, UPI, wallet).
Secure transaction handling.
Mock payment integration for testing.
Tech Stack
Frontend
React: For building an interactive and dynamic user interface.
Next.js: For server-side rendering and improving performance.
Backend
Express.js: For building the RESTful API to handle business logic.
Mongoose: For managing the MongoDB database and creating schemas.
Database
MongoDB: To store user information, product data, orders, and payment records.
Milestones
Milestone 1: Setup Development Environment
Installed all necessary tools and dependencies for the MERN stack.
Understood server-client interaction in a full-stack application.
Created a basic Node.js and Express server.
Milestone 2: Project Structure & Basic Frontend
Designed and implemented a structured folder hierarchy.
Set up React for the frontend and Express.js for the backend.
Configured Tailwind CSS for styling.
Added optional extensions (Prettier, ESLint) for development efficiency.
Built a functional and styled Login Page.
Milestone 3: Backend Setup
Created dedicated folders for organizing backend code.
Configured a Node.js server using Express.
Established a connection to MongoDB.
Implemented basic error handling.
Milestone 4: User Model & File Uploads
Created a User Model with a defined schema.
Developed a User Controller for user-related operations.
Configured Multer for handling file uploads.
Milestone 5: Signup Page & Validation
Created a Sign-Up Page in React.
Implemented form validation:
Name (required)
Email (valid format required)
Password (minimum 2 characters)
Password Confirmation (must match password)
Used React Router for navigation.
Milestone 6: User Registration & Authentication
Implemented a /create-user endpoint to store user details.
Used bcrypt.js to hash passwords before saving them to the database.
Implemented centralized error handling.
Integrated an email notification system (optional).
Generated JWT tokens upon successful login.
Milestone 7: Login API
Created a login endpoint accepting email/password.
Verified user credentials and validated passwords using bcrypt.
Generated a JWT token for authentication.
Implemented error handling for invalid credentials and server errors.
Milestone 8: Creating a Home Page
Designed a responsive homepage layout.
Implemented a grid layout for displaying product cards.
Ensured responsiveness for different screen sizes.
Milestone 9: Creating a Product Form
Created a form to input product details.
Allowed users to upload multiple product images.
Saved the entered details in the database.
Milestone 10: Product Schema & API Endpoint
Created a Mongoose schema for products.
Developed a POST endpoint to validate and store product data in MongoDB.
Milestone 11: Fetch & Display Products
Created an API endpoint to fetch all products from the database.
Implemented a frontend function to fetch and display product data dynamically.
Used useState and useEffect to manage the data lifecycle.
Milestone 12: Fetch & Display Filtered Products
Created an API endpoint to fetch products based on the user's email.
Implemented frontend logic to request and display filtered products.
Ensured efficient state management using React hooks.
Milestone 13:- Edit Product Functionality
Created a PUT API endpoint to update product details in MongoDB.
Added an Edit button on the product card.
Implemented auto-filled form for editing existing product details.
Connected frontend with backend to send PUT requests.
Handled errors and ensured data validation.
Milestone 14:- Edit & Delete Product Functionality
Created a PUT API endpoint to update product details in MongoDB.
Added an Edit button on the product card.
Implemented auto-filled form for editing existing product details.
Connected frontend with backend to send PUT requests.
Handled errors and ensured data validation.
Created a DELETE API endpoint to remove products from MongoDB.
Added a Delete button to the product card.
Integrated frontend with backend to send DELETE requests.
Milestone 15 - Creating a Navbar Component
Create a New Nav Component
The Navbar should include links to the following pages:
Home
My Products
Add Product
Cart
Navbar is responsive and adapts to different screen sizes.
Add Navbar to All Pages
Import and integrate the Nav component into all pages.
Ensure smooth navigation between different sections of the application.
Make the Navigation Smooth & User-Friendly
Use React Router for handling navigation.
Implement active link highlighting for better UX.
Optimize the layout to be mobile-friendly.
Milestone 16 - Creating a Product Info Page
Create a New Product Info Page
The page should display detailed information about a product.
Include product name, image, price, and description.
Add a Quantity Selector
Allow users to select the desired quantity of the product.
Ensure the quantity selection updates dynamically.
Implement the Add to Cart Button
Add a button that allows users to add the selected quantity of the product to their cart.
Ensure smooth user interaction and feedback after adding to cart.
Milestone 17: Add Products to Cart & Store in Database
Created the Cart Schema: Defined a schema to store cart products linked to users. Implemented an API endpoint: Developed a backend route to handle adding products to the cart. Stored Cart Data: Successfully saved product details in the database under the user's cart.
 main
