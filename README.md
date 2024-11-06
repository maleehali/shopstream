# E-commerce Back End Starter Code
# E-Commerce Back End

This project is a back-end application for an e-commerce site built with Node.js, Express.js, Sequelize, and PostgreSQL. It provides a functional API that supports basic CRUD operations for product categories, products, and tags, simulating the back-end functionality of a typical e-commerce platform.

## Table of Contents
- [User Story](#user-story)
- [Acceptance Criteria](#acceptance-criteria)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Routes](#api-routes)
- [Walkthrough Video](#walkthrough-video)
- [Credits](#credits)
- [License](#license)

---

## User Story
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies

## Acceptance Criteria

The application meets the following criteria:
1. A working Express.js API.
2. Database connection using Sequelize with environment variables for security.
3. Database schema and seed commands run without issues.
4. Server start command initiates Sequelize model synchronization with the PostgreSQL database.
5. Insomnia Core shows the formatted JSON data for all categories, products, and tags.
6. Insomnia Core successfully demonstrates create, update, and delete operations.

## Technologies Used

- Node.js
- Express.js
- Sequelize ORM
- PostgreSQL
- Dotenv for environment variable management

---

## Installation

1. **Clone the Repository**: 
    ```bash
    git clone https://github.com/maleehali/shopstream.git
    ```

2. **Install Dependencies**:
    ```bash
    npm install
    ```

3. **Set Up Environment Variables**:
   - Create a `.env` file at the root of your project with the following contents:
     ```
     DB_NAME=ecommerce_db
     DB_USER=yourPostgresUsername
     DB_PASSWORD=yourPostgresPassword
     ```

4. **Create the Database Schema**:
    ```bash
    psql -U postgres -f db/schema.sql
    ```

5. **Seed the Database**:
    ```bash
    npm run seed
    ```

6. **Start the Server**:
    ```bash
    npm start
    ```

---

## Usage

1. Use Insomnia Core or any API client to test the API routes.
2. Access different API endpoints (see [API Routes](#api-routes)) to perform CRUD operations on categories, products, and tags.

---

## API Routes

### Categories
- **GET** `/api/categories` - Get all categories
- **GET** `/api/categories/:id` - Get category by ID
- **POST** `/api/categories` - Create a new category
- **PUT** `/api/categories/:id` - Update a category by ID
- **DELETE** `/api/categories/:id` - Delete a category by ID

### Products
- **GET** `/api/products` - Get all products
- **GET** `/api/products/:id` - Get product by ID
- **POST** `/api/products` - Create a new product
- **PUT** `/api/products/:id` - Update a product by ID
- **DELETE** `/api/products/:id` - Delete a product by ID

### Tags
- **GET** `/api/tags` - Get all tags
- **GET** `/api/tags/:id` - Get tag by ID
- **POST** `/api/tags` - Create a new tag
- **PUT** `/api/tags/:id` - Update a tag by ID
- **DELETE** `/api/tags/:id` - Delete a tag by ID

---

## Walkthrough Video

Here is a walkthrough video demonstrating the functionality of the application, including the database setup, seeding, and testing of all API routes:
[Walkthrough Video Link](https://drive.google.com/file/d/1n3sUKb73A2ZNvqw4hXL_NE3TVrbRNili/view?usp=sharing)

---

## License

This project is licensed under the MIT License.

