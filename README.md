# To-Do-List-API-Testing-using-Postman
This repository contains a simple To-Do-List application APIs built with Node.js and Express.js. It allows users to manage a list of tasks with endpoints to perform (Create, Read, Update, Delete) operations. Here's a brief description of its endpoints:

**GET /todos**

Description: Retrieves the list of all to-do items.
Response: An array of to-do objects, each containing an "id", "title", and "completed" status.

**GET /todos/:id**

Description: Fetches a specific to-do item by its ID.
Response: A single to-do object if found, or a 404 status with a "Todo not found" message if the ID does not exist.

**POST /todos**

Description: Adds a new to-do item.
Request Body: JSON object with a "title" field (optional "completed" field defaults to false).
Response: The newly created to-do object with a unique "id".

**PUT /todos/:id**

Description: Updates an existing to-do item by ID.
Request Body: JSON object with fields to be updated ("id", "title" and "completed").
Response: The updated to-do object if found, or a 404 status with a "Todo not found" message if the ID does not exist.

**DELETE /todos/:id**

Description: Deletes a to-do item by ID.
Response: A 204 status indicating successful deletion, or a 404 status with a "Todo not found" message if the ID does not exist.

## API Testing

I have implemented automated tests using Postman. These tests cover key API endpoints, validating correct responses, status codes, and error handling for various user scenarios. The tests include checking the creation, retrieval, updating, and deletion of to do items. You can find the collection of Postman tests in the Postman Collection folder, ready to be imported and executed to validate the functionality of the API.

**note:** inorder to run these collection you will need to do the following:

+ Clone the project files andensure all dependecies are present, then run the project using the command "npm start" to build the application.
+ Retrive the local host url to use it in Postman.
+ Download Postman desktop agent, then import the collection and update the url.
