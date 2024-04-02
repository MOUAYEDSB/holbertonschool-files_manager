# holbertonschool-files_manager

<img src="image/images.jpg">

This project is a back-end application aimed at providing a platform for users to upload, manage, and view files. It encompasses user authentication, file storage in MongoDB, temporary data storage in Redis, background processing for generating thumbnails of images, and various API endpoints for file management.

## Project Overview

The main functionalities of the Files Manager API include:

- User authentication via tokens
- Listing all files
- Uploading new files
- Changing permissions of files
- Viewing files
- Generating thumbnails for images

## Technologies Used

The project is built using the following technologies and tools:

- Node.js
- Express.js
- MongoDB
- Redis
- Bull (for background processing)
- ESLint (for linting)
- Other relevant Node.js libraries

## Installation

To run the project locally, follow these steps:

1. Clone this repository to your local machine.
2. Navigate to the project directory.
3. Run `npm install` to install the necessary dependencies.
4. Set up the required environment variables, such as `PORT`, `DB_HOST`, `DB_PORT`, `DB_DATABASE`, and `FOLDER_PATH`.
5. Run `npm start` to start the server.

## Usage

Once the server is running, you can interact with the API using tools like cURL or Postman. Here are some example requests:

- **GET /status**: Check the status of Redis and MongoDB.
- **GET /stats**: Get statistics about the number of users and files in the database.
- **POST /users**: Create a new user.
- **GET /connect**: Authenticate a user and generate a token.
- **GET /disconnect**: Sign out a user and invalidate the token.
- **POST /files**: Upload a new file.
- **GET /files/:id**: Retrieve information about a specific file.
- **PUT /files/:id/publish**: Publish a file.
- **PUT /files/:id/unpublish**: Unpublish a file.
- **GET /files/:id/data**: Get the content of a file.

## Learning Objectives

By working on this project, you will gain experience with the following concepts:

- Creating an API with Express.js
- Implementing user authentication
- Storing data in MongoDB
- Managing temporary data with Redis
- Setting up and using background workers for processing tasks

## Authors

- [Mouayed sabbagh](https://github.com/MOUAYEDSB)