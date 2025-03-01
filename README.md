# 📝 Node.js Task Manager API

This is a **simple RESTful API** built with **Node.js and Express.js**. It allows users to **manage tasks** by adding, retrieving, and deleting them.

---

##  Features

 Get all tasks  
 Add a new task  
 Delete a task by ID  
 Uses an **in-memory array** (no database required)  
 Proper **error handling** for invalid requests  

---

##  Installation & Setup
```sh
 1️ Clone the Repository
Run the following command to clone the repository and navigate into the project folder:

git clone https://github.com/yourusername/node-api-task.git
cd node-api-task
2️ Install Dependencies
Install the required Node.js dependencies:
npm install

▶ Running the API
Start the server using:
npm start
The API will now run on http://localhost:3000.

 API Endpoints
 1️ Get All Tasks
Endpoint: GET /api/tasks
Description: Returns an array of tasks.
 Example Response:

json
{
    { "id": 1, "name": "Buy groceries", "completed": false },
    { "id": 2, "name": "Do laundry", "completed": true }
}

 2️ Add a New Task
Endpoint: POST /api/tasks
Description: Adds a new task.
Request Body (JSON Format):
json
{ "name": "New Task" }
 Example Response:
json
{
"id": 3, 
"name": "New Task",
"completed": false 
}

 3️ Delete a Task
Endpoint: DELETE /api/tasks/:id
Description: Deletes a task by its ID.
 Example Request:
DELETE /api/tasks/1
 Example Response:
json
{ "message": "Task deleted successfully" }

 Technologies Used
Node.js
Express.js
JavaScript (ES6)
 Notes
No database is used—tasks are stored in memory and reset when the server restarts.
Use Postman or any API testing tool to interact with the API.
