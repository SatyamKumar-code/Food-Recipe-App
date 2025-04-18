# Food Recipe Application

The Food Recipe Application is a full-stack web application that allows users to browse, add, and manage food recipes. It includes features like user authentication, recipe sharing, and a visually appealing interface.

## Features

- **User Authentication**: Sign up and log in to access personalized features.
- **Recipe Management**: Add, edit, and view recipes with images, ingredients, and instructions.
- **Favorites**: Mark recipes as favorites for quick access.
- **Responsive Design**: Optimized for both desktop and mobile devices.
- **Secure API**: Backend API with token-based authentication.

## Tech Stack

### Frontend
- React
- React Router
- Styled Components
- Vite

### Backend
- Node.js
- Express.js
- MongoDB
- Multer (for file uploads)
- JWT (for authentication)

## Installation

### Prerequisites
- Node.js and npm installed
- MongoDB instance running locally or in the cloud

### Steps
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd FoodRecipe
   ```

2. Install dependencies for both frontend and backend:
   ```bash
   cd frontend
   npm install
   cd ../backend
   npm install
   ```

3. Set up environment variables:
   - Create a `.env` file in the `backend` directory with the following:
     ```
     MONGODB_URI=<your-mongodb-uri>
     SECRET_KEY=<your-secret-key>
     PORT=5000
     ```

4. Start the backend server:
   ```bash
   cd backend
   node server.js
   ```

5. Start the frontend development server:
   ```bash
   cd ../food-blog-app
   npm run dev
   ```

6. Open the application in your browser at `http://localhost:5173`.

## Usage

- **Browse Recipes**: View all recipes on the homepage.
- **Add Recipes**: Click "Share your recipe" to add a new recipe (requires login).
- **My Recipes**: View recipes created by you.
- **Favorites**: Access your favorite recipes.

## API Endpoints

### User Routes
- `POST /signUp`: Register a new user.
- `POST /login`: Log in an existing user.
- `GET /user/:id`: Get user details by ID.

### Recipe Routes
- `GET /recipes`: Get all recipes.
- `GET /recipes/:id`: Get a single recipe by ID.
- `POST /recipes`: Add a new recipe (requires authentication).
- `PUT /recipes/:id`: Edit a recipe by ID.
- `DELETE /recipes/:id`: Delete a recipe by ID.
- `POST /recipes/favorite/:id`: Add a recipe to favorites (requires authentication).
- `GET /recipes/favorites`: Get all favorite recipes (requires authentication).
- `GET /recipes/user/:id`: Get all recipes created by a specific user.
## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.
