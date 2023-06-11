## BACK-END-E-COMMERCE
This project is a functional Express.js API integrated with Sequelize, a popular Node.js ORM (Object-Relational Mapping) library for interacting with databases. It provides a set of routes for managing categories, products, and tags, allowing users to perform CRUD (Create, Read, Update, Delete) operations on a MySQL database.

## Demo Video (Insomnia)
https://drive.google.com/file/d/10N20U4BeVCRvRGbnW_WLZb7Z7bPACbDd/view

## Prerequisites
Before running this project, ensure you have the following:

1. Node.js installed on your machine.
2. MySQL server installed and running.
3. An API client tool (e.g., Insomnia Core, Postman) for testing the API routes.
## Getting Started
To set up and run the project locally, please follow these steps:

1. Clone the repository:

bash
Copy code
git clone [repository URL]
Navigate to the project directory:

bash
Copy code
cd [project directory]
Install dependencies:

bash
Copy code
npm install
Create an environment variable file named .env in the root directory of the project and add the following variables:

bash
Copy code
DB_NAME=[your_database_name]
DB_USER=[your_mysql_username]
DB_PASSWORD=[your_mysql_password]
Run the database schema and seed commands to create the development database and populate it with test data:

bash
Copy code
npm run db:reset
Start the server and sync the Sequelize models with the MySQL database:

bash
Copy code
npm start
Once the server is running, you can use an API client tool (e.g., Insomnia Core) to interact with the API routes.

## API Routes
1. Categories
    GET /api/categories: Retrieve all categories.

    GET /api/categories/:id: Retrieve a specific category by ID.

    POST /api/categories: Create a new category.

    PUT /api/categories/:id: Update an existing category.

    DELETE /api/categories/:id: Delete a category.

2. Products
    GET /api/products: Retrieve all products.

    GET /api/products/:id: Retrieve a specific product by ID.

    POST /api/products: Create a new product.

    PUT /api/products/:id: Update an existing product.

    DELETE /api/products/:id: Delete a product.

3. Tags
    GET /api/tags: Retrieve all tags.

    GET /api/tags/:id: Retrieve a specific tag by ID.

    POST /api/tags: Create a new tag.

    PUT /api/tags/:id: Update an existing tag.

    DELETE /api/tags/:id: Delete a tag.

Please note that :id should be replaced with the corresponding ID of the category, product, or tag you wish to access or modify.

## Testing API Routes
Using your preferred API client tool (e.g., Insomnia Core, Postman), you can perform the following actions:

    Send GET requests to retrieve data from the API routes mentioned above.
    Send POST requests to create new data.
    Send PUT requests to update existing data.
    Send DELETE requests to delete data.
    Ensure you have the correct route URL and provide the required data in the request body or parameters based on the route's documentation.

## Contributing
Contributions to this project are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License.