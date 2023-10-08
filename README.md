# Angelin_E_Commerce

## Summary
This project involves building the back end for an e-commerce site The application allows users to manage product categories, products, and tags of an internet retail company.

## Video Walkthrough
https://www.dropbox.com/scl/fi/dnqhlc8qjodkfhxq2k52b/Angelin_E_Commerce_WalkThrough.webm?rlkey=nn1kutjl1bs4wt0s8hfz3wzie&dl=0

## Functionality
### Database Setup and Seeding
1. The application connects to a MySQL database using Sequelize ORM.
2. The database is initialized and seeded with test data using schema and seed commands.

### API Routes
1. **GET Routes**
   - `/api/categories`: Get all categories in a formatted JSON response.
   - `/api/products`: Get all products in a formatted JSON response.
   - `/api/tags`: Get all tags in a formatted JSON response.

2. **POST Routes**
   - `/api/categories`: Create a new category by providing category details in the request body.
   - `/api/products`: Create a new product by providing product details in the request body.
   - `/api/tags`: Create a new tag by providing tag details in the request body.

3. **PUT Routes**
   - `/api/categories/:id`: Update an existing category by providing category details in the request body.
   - `/api/products/:id`: Update an existing product by providing product details in the request body.
   - `/api/tags/:id`: Update an existing tag by providing tag details in the request body.

4. **DELETE Routes**
   - `/api/categories/:id`: Delete an existing category by specifying its ID.
   - `/api/products/:id`: Delete an existing product by specifying its ID.
   - `/api/tags/:id`: Delete an existing tag by specifying its ID.


## Database Models
The database contains the following four models, each with specific requirements:
1. **Category** (Fields: id, category_name)
2. **Product** (Fields: id, product_name, price, stock, category_id)
3. **Tag** (Fields: id, tag_name)
4. **ProductTag** (Fields: id, product_id, tag_id)


## Deployment Steps
1. Set up your own repository with the starter code, and clone the repository to your local machine.
2. Navigate to the project directory
3. Install the required dependencies using `npm install`.
5. Create a `.env` file and add your database name, MySQL username, and MySQL password.
4. Execute schema and seed commands to create and seed the development database.
5. Run the application using `node server.js`.
6. Use tools like Insomnia to test API GET, POST, PUT, and DELETE routes for categories, products, and tags.

## Outside Sources
- https://www.freecodecamp.org/news/what-is-an-orm-the-meaning-of-object-relational-mapping-database-tools/
- https://www.theserverside.com/definition/object-relational-mapping-ORM
- Tutoring session