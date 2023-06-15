# ProjectX
User Authentication REST API
This project implements a REST API for user authentication, including endpoints for user login and signup functionality. It uses Java, Spring Boot, and H2 database.

Prerequisites
Java Development Kit (JDK) 8 or higher
Maven
Getting Started

Clone the repository:
Copy code
git clone https://github.com/Yash5chaubey/ProjectX.git

Navigate to the project directory:
Copy code
cd ProjectX

Build the project:
Copy code
mvn clean install

Run the application:
Copy code
mvn spring-boot:run
The application will start running on http://localhost:8080.

API Endpoints

Signup
Endpoint: POST /api/signup
Description: Creates a new user account.
Request Body:
username: User's username (string)
password: User's password (string)
Response:
200 OK: Signup successful
409 Conflict: Username already 

Login
Endpoint: POST /api/login
Description: Authenticates a user and generates a web token.
Request Body:
username: User's username (string)
password: User's password (string)
Response:
200 OK: Web token generated successfully
401 Unauthorized: Invalid username or password

Configuration
The project uses an H2 in-memory database by default. You can configure the database connection, application port, and other properties in the application.properties file.

Dependencies
Spring Boot Starter Web
Spring Boot Starter Data JPA
H2 Database
JSON Web Token (JWT)

Contributing
Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.
