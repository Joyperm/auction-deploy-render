# Summary

### Component Hierarchy
- **App**:
  - Root component that sets up routes and provides global context.

- **Header**:
  - Contains the `Navbar` and `DarkModeToggle` components.

- **Navbar**:
  - Navigation links to different pages.

- **DarkModeToggle**:
  - Toggles between light and dark modes.

- **Routes**:
  - Home (`Products`)
  - Add Product (`ProductForm`)
  - About Us (`AboutUs`)
  - Not Found (`NotFound`)

#### Component Map diagram
![image](https://github.com/user-attachments/assets/08c95bce-5c46-4ae0-ab0a-df07998797e2)

## API structure
- **Main Server File (server.js or index.js)**
  - Sets up an Express server.
  - Connects to a MongoDB database using Mongoose.
  - Configures middleware, including CORS and JSON parsing.
  -  Defines routes for the API, delegating product-related routes to a separate router (productRouter).
- **Product Controller (productControllers.js)**
  - Contains functions to handle CRUD operations for products:
    - getProducts: Fetches all products.
    - getProduct: Fetches a single product by ID.
    - createProduct: Creates a new product.
    - deleteProduct: Deletes a product by ID.
    - updateProduct: Updates a product by ID.
    - updateProductPrice: Updates only the price of a product by ID.
    - getLikes: Increases the like count of a product by ID.

- **Product Model (productsModel.js)**
  - Defines the structure of a product document in the MongoDB database.
  - Uses Mongoose schema to specify fields and their types (e.g., name, image, initialPrice, newPrice, description, tag, likes).

- **Product Router (products.js)**
  - Sets up routes for the product-related endpoints.
  - Associates each route with the corresponding controller function.

## Features and technologies used
- **Features Implemented**: Product listing, bidding, search, filtering, and love rating system.
- **Technologies Used**: React, Node.js, Express, MongoDB Atlas.
- **API**: Integrated own API with product data.
- **Deployment**: Front-end and back-end on render.

## Video Demonstration
- [Watch the demo video]
(https://drive.google.com/file/d/1ATcTYjmjmijsonTCJt43HuVwlkXim_Ro/view?usp=sharing)

## References
- [GitHub Repository-backend](https://github.com/NavneetBrar27/backend.git )
- [GitHub Repository-frontend](https://github.com/NavneetBrar27/frontend.git )
- [Link to the site](https://frontend-3-9u06.onrender.com/products)

## Example demo
- **Home page**
- ![image](https://github.com/user-attachments/assets/dc2bc31d-b645-4453-8cf8-940c6328724d) 

- **Home page Dark mode**
- ![image](https://github.com/user-attachments/assets/f71d9c65-6a48-40ee-ae57-78ec10171435)

 
- **Add new Product page**
- ![image](https://github.com/user-attachments/assets/cb01e21c-6039-4865-9392-5b7dac0e5c95)

 
- **About us page**
- ![image](https://github.com/user-attachments/assets/faeab088-ab15-4004-ac25-05ccadf5280d)

- **Bidding**
- ![bidding](https://github.com/user-attachments/assets/1acb7286-989e-4f92-822e-e57de414dc22)


- **Adding Product**
- ![addProduct](https://github.com/user-attachments/assets/945bc4bd-0ce0-4e61-be90-d27da25eaa34)


- **Deleting Product**
- ![delete](https://github.com/user-attachments/assets/db847668-e85c-4091-9f23-42a439b25a8e)


- **Search Product**
- ![searchProduct](https://github.com/user-attachments/assets/d7800eab-61e5-4123-8b12-af92d90da0ad)

- **Love Product**
- ![likeProduct](https://github.com/user-attachments/assets/5d9b7dc7-7e28-4ee1-9adf-9131a7427e4e)


 

- **Page not found**
- ![image](https://github.com/user-attachments/assets/1b4a15f9-2950-456a-96c9-8bcb46c629f3)
