# Forum App

Forum App is a web application built with ejs and style with vanilla css. 
It provides a user-friendly interface to Create and manage three distinct collections: 
"User," "Post," and "Comments" to handle different data types. It describe the relationship between 
posts and comments within the application's data structure and Map application functionality to specific 
routes and control logic using controllers.

## Features

- User authentication: Register and log in to access the application.
- Task management: Make a Post, and Comments.
- Describe the relationship between posts and comments within the application's data structure
- Map application functionality to specific routes and control logic using controllers..

## Installation

To run the Forum App Frontend locally, follow these steps:

1. Clone the repository from GitHub:

   ```bash
   git clone https://github.com/tosmel2/forum-app.git
   ```

2. Navigate to the project directory:

   ```bash
   cd forum-app
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Start the development server:

   ```bash
   node app.js
   ```

5. Access the application in your browser at `http://localhost:3000`.

## Usage

### User Authentication

- **Register**: Click on the "Register" button and fill in the required details to create a new account.
- **Log In**: Enter your email/username and password, then click on the "Log In" button to access the application.

### Task Management

- **Create Post**: Click on the "Post" button, fill in the post details, and click "Submit" to create a new post.
- **Comment on Post**: Click on the comment button, to make a comment on the post.

### Environment variables
db_connection="mongodb+srv://username:<yourpassword>@forumcluster.i7p4r5g.mongodb.net/?retryWrites=true&w=majority&appName=ForumCluster"
PORT=3000
SESSION_SECRET='topsecret'

## Dependencies

- bcryptjs: Hashing algorithm to create hashes for passwords to store them in case of a data breach.
- body-parser: Node.js body parsing middleware.
- dotenv: Loads environment variables from .env file.
- ejs: Embedded JavaScript templates.
- express: minimalist web framework for Node.js.
- express-session: Simple session middleware for express.
- mongoose:  MongoDB object modeling tool designed to work in an asynchronous environment..

## Folder Structure

```
FORUM-APP/
├── controllers/            # Application logic
|   ├── authController.js   # auth application logic
|   ├── indexController.js  # index application logic
|   ├── postController.js   # post application logic
├── models/                 # Schemas of database
|   ├── CommentModel.js     # Schemas of comment model
|   ├── PostModel.js        # Schemas of post model
|   ├── UserModel.js        # Schemas of user model
├── public/                 # Static assets
|   ├── styles.css          # Global styles
├── routes/                 # The subroutes
|   ├── authHandling.js     # route for authentication
|   ├── indexHandling.js    # route for index
|   ├── postHandling.js     # route for post
├── views/                  # The EJS files that will be server-rendered to the front end
|   ├── components/         # Reusable components
|       ├── dashboard.ejs   # dashboard EJS file
|       ├── index.ejs       # index EJS file
|       ├── login.ejs       # login EJS file
|       ├── post_id.ejs     # post ID EJS file
|       ├── post.ejs        # post EJS file
|       ├── register.ejs    # register EJS file
├── .env                    # environment variables
├── .gitignore              # Git ignore file
├── app.js                  # Entry point
├── package.json            # npm package file
└── README.md               # Project README
```




