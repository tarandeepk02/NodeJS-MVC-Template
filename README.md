# Node.js MVC Template

This is a basic Node.js template project structured using the MVC (Model-View-Controller) design pattern. It provides a clean starting point for building scalable Node.js applications. The template uses Express.js, EJS for templating, and a basic file structure to separate the logic of models, views, and controllers.

## Features

- **MVC Architecture**: Clean separation of concerns with Models, Views, and Controllers.
- **Express.js**: A fast, unopinionated, minimalist web framework for Node.js.
- **EJS**: A simple templating engine for rendering HTML views.
- **Basic Authentication**: Optional integration of user authentication.
- **Database Integration**: MongoDB support via Mongoose for data storage.
- **RESTful API**: A foundation for creating REST APIs alongside web pages.
- **Environment Configuration**: Support for environment variables with `dotenv`.

## Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org) (v12.x or higher)
- [npm](https://www.npmjs.com/) (v6.x or higher)

## Installation

1. Clone the repository:
    ```
    git clone https://github.com/yourusername/NodeJS-MVC-Template.git
    cd NodeJS-MVC-Template
    ```

2. Install the required dependencies:
    ```
    npm install
    ```

3. Configure MongoDB: Update database credentials in models/config/config.js
    ```
    (() => {
     const config = {}
     config.SERVER = ''
     config.USERNAME = ''
     config.PASSOWRD = ''
     config.DATABASE = ''
     module.exports = config`
     })()
    ```
4. Run the application:
    ```
    npm start
    ```

5. The application should now be running on http://localhost:3000

## Project Structure

The project follows a typical MVC structure:

### Key Files

- **`server.js`**: The main entry point where the Express server is set up.
- **`controllers/`**: Contains the logic to handle HTTP requests.
- **`models/`**: Contains the database models used by Mongoose
- **`views/`**: Contains templates for rendering HTML

## Usage

1. **Add New Models**: Create a new file in the `models` directory to define a new Mongoose model. For example, for a `Post` model, create `models/postModel.js`.

2. **Add New Controllers**: Create a new file in the `controllers` directory to handle business logic. For example, for a `Post` controller, create `controllers/postController.js`.

3. **Bootstrap in Views**: All the views are rendered with a layout that includes Bootstrap's CSS and JS files for responsive design. Modify the `views/post.html` file to update the layout or add more Bootstrap components.



