# shop-plus-plus: A MERN-Stack E-commerce Application


## Features

- **Product Management:**
    - View a list of products.
    - View detailed product information.
    - Add products to the shopping cart.

- **Shopping Cart:**
    - View items in the shopping cart.
    - Remove items from the cart.
    - Calculate total amount of items in the cart.

- **Checkout Process:**
    - Enter billing, shipping, and payment information.
    - Simulate the order creation process on the backend.
    - Receive confirmation of order success.

## Technologies Used

- **Frontend:**
    - React.js
    - Material-UI for styling
    - Axios for API requests
    - `react-credit-cards-2` for credit card visualization

- **Backend:**
    - Node.js
    - Express.js
    - MongoDB (with Mongoose ODM)
    - Axios for external API requests
    - Nodemon for server hot-reloading

- **Development Tools:**
    - VSCODE
    - Postman (for API testing)
    - Git (version control)
    - npm (package manager)


## Getting Started

### Prerequisites

Before running this project, ensure you have the following installed:

- Node.js (with npm)
- MongoDB (with either local or remote instance)
- Git

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/PalakDubey27/Shop-plus-plus.git
   cd Shop-plus-plus
   ```

2. Install project dependencies:
   ```bash
   # Install server dependencies
   cd backend
   npm install

   # Install client (frontend) dependencies
   cd ..
   npm install
   ```
   
3. Set up the backend:

   - Create a `.env` file in the `backend/` directory and add the following environment variables:
     ```
     MONGO_URI=mongodb://localhost:27017/Ecommerce-Products
     ```
 
    - Ensure that your MongoDB server is running. If you're using Mac, you can start the MongoDB server with the following command:
     ```bash
     brew services start mongodb-community
     ``` 

   - Seed the database with sample data:
     ```bash
     cd backend/seed
     node productSeeds.js dev
     ```
     
   - Run the backend server: (first `cd` into the backend directory)
     ```bash
     cd ..
     npm start
     ``` 
     
4. Set up the frontend:
   - First, `cd` into the `root` directory if you are not already there:
     ```bash
     cd ..
     ```
     Or
        ```bash
        cd Shop-plus-plus
        ```
   - Start the frontend development server:
     ```bash
     npm start
     ```

## Running the Application

- Open your browser and navigate to `http://localhost:3000` to view the application.

