# Employee-Management-RESTAPI
Features

CRUD Operations: Create, Read, Update, and Delete employee records.

Layered Architecture: Controller → Service → Repository for maintainability.

API Documentation: Integrated Swagger UI for interactive API testing.

Containerization: Docker support for seamless setup and deployment.

Testing:

JUnit for unit testing.

Cucumber for BDD-style testing against real-world scenarios.

Tech Stack

Backend: Spring Boot (REST API, Spring Data JPA)

Database: MySQL

Containerization: Docker

Testing: JUnit, Cucumber

API Documentation: Swagger

⚙️ Setup & Installation
Clone the Repository
git clone https://github.com/YukthaDoddaRangappa/Employee-Management-RESTAPI
cd employee-management-system

Configure Database (MySQL)

Update application.properties with your MySQL credentials:

spring.datasource.url=jdbc:mysql://localhost:3306/employee_db
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update

Run with Docker
# Build Docker image
docker build -t employee-management-system .

# Run container
docker run -p 8080:8080 employee-management-system

 Running Tests
Unit Tests (JUnit)
mvn test

BDD Tests (Cucumber)
mvn verify

API Endpoints
Method	Endpoint	Description
GET	/api/employees	Fetch all employees
GET	/api/employees/{id}	Fetch employee by ID
POST	/api/employees	Create new employee
PUT	/api/employees/{id}	Update employee details
DELETE	/api/employees/{id}	Delete employee by ID
 Future Enhancements

Add role-based authentication with Spring Security.

Implement pagination and filtering for employees.

Add CI/CD pipeline with GitHub Actions.

Author

Developed by Yuktha D

Author
Yuktha D - https://github.com/YukthaDoddaRangappa?tab=repositories

Support
If you have any questions or issues, please open an issue on GitHub or contact me at [yuktha.drangappa@gmail.com].


