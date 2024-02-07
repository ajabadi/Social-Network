# Social-Network

## Description

This project is designed to demonstrate the capabilities of a NoSQL database in supporting a social network web application. Utilizing MongoDB, a popular choice for handling large amounts of unstructured data, the API enables users to share thoughts, react to friends' thoughts, and manage a friend list. The project leverages Express.js for routing, MongoDB for the database, and Mongoose ODM for data modeling. This API exemplifies the foundational technologies behind many social networking platforms.

## User Story

AS A social media startup, created an API for the social network that uses a NoSQL database, so that the website can handle large amounts of unstructured data

## Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose ODM
- (Optional) A JavaScript date library of your choice for formatting timestamps

## Installation

1. Clone the repository to your local machine.
2. Install Node.js and MongoDB if you haven't already.
3. Navigate to the project directory and run `npm install` to install dependencies.
4. Ensure MongoDB is running on your system.
5. Use `npm start` to initiate the server.

## Usage

The API supports the following routes:

### Users

- **GET /api/users**: Retrieve all users.
- **GET /api/users/:id**: Retrieve a single user by its _id along with populated thought and friend data.
- **POST /api/users**: Create a new user.
- **PUT /api/users/:id**: Update a user by its _id.
- **DELETE /api/users/:id**: Delete a user by its _id.

### Friends

- **POST /api/users/:userId/friends/:friendId**: Add a new friend to a user's friend list.
- **DELETE /api/users/:userId/friends/:friendId**: Remove a friend from a user's friend list.

### Thoughts

- **GET /api/thoughts**: Get all thoughts.
- **GET /api/thoughts/:id**: Get a single thought by its _id.
- **POST /api/thoughts**: Create a new thought.
- **PUT /api/thoughts/:id**: Update a thought by its _id.
- **DELETE /api/thoughts/:id**: Delete a thought by its _id.

### Reactions

- **POST /api/thoughts/:thoughtId/reactions**: Create a reaction for a thought.
- **DELETE /api/thoughts/:thoughtId/reactions**: Delete a reaction from a thought.

## Walkthrough Video
(Walkthrough video)[https://app.screencastify.com/v3/watch/Iam2xEYgtGwaTvp2juJl] for the user

<img width="1228" alt="Screen Shot 2024-02-06 at 18 37 59" src="https://github.com/ajabadi/Social-Network/assets/145517793/91f82488-6a37-4ca8-8e5b-dc083e887edc">

