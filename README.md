
Curd REST API
This project is a simple Curd REST API implemented in Java with Spring Boot and MongoDB. It provides basic CRUD operations for managing tasks.

Prerequisites
Before running this application, make sure you have the following installed:

Java 17 or later
Maven
MongoDB
Getting Started
To run this application locally, follow these steps:

Clone this repository:

bash
Copy code
git clone https://github.com/animal831/curdoperations.git
Navigate into the project directory:

bash
Copy code
cd curdoperations
Build the application using Maven:

bash
Copy code
mvn clean package
Run the application:

bash
Copy code
java -jar target/curdoperations-0.0.1-SNAPSHOT.jar
The application will start running at http://localhost:8080.

API Endpoints
GET /api/tasks: Retrieve all tasks.
GET /api/tasks/{id}: Retrieve a task by ID.
POST /api/tasks: Create a new task.
Request body:
json
Copy code
{
  "name": "Task Name",
  "description": "Task Description"
}
PUT /api/tasks/{id}: Update an existing task by ID.
Request body:
json
Copy code
{
  "id": "task-id",
  "name": "Updated Task Name",
  "description": "Updated Task Description"
}
DELETE /api/tasks/{id}: Delete a task by ID.
Security
This application uses basic authentication with username admin and password sanju to secure the API endpoints. Make sure to change the credentials and consider using more secure authentication methods for production.

Contributing
Contributions are welcome! Feel free to fork this repository, make your changes, and submit a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.
