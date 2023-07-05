# follow-service
The Follow Service is a microservice in the Instagram clone application that handles user follow functionality. It allows users to follow and unfollow other users, manage follow requests, and retrieve followers and followed users.
## Features
- Retrieve all follows
- Retrieve follows for a specific user
- Retrieve followers for a specific user
- Add a follow relationship between users
- Accept follow requests
- Unfollow a user
- Retrieve follow requests for a user
## Technologies Used
- Java 17
- Spring Boot 3.1.0
- Maven 4.0.0
- PostgreSQL 15.3
## Dependencies

- [Spring Boot] 
- [Spring Web]
- [Spring Data JPA]
- [postgresql]
- [Spring Cloud]
- [Spring Cloud OpenFeign]

## Getting Started
These instructions will get you a copy of the Follow Service up and running on your local machine for development and testing purposes.

### Prerequisites

- [Java SE Development Kit 17.0.5] (https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
- [Maven 4.0.0] (https://maven.apache.org/install.html)
- [Spring Boot CLI] (https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#getting-started-installing-the-cli) (Optional)

### Installation
1. Clone the repository:
```bash
git clone <repository-url>
```
2. Navigate to the project directory::
```bash
cd follow-service
```
3. Open the application.properties file and configure the database connection details:
```
spring.datasource.url=jdbc:mysql://localhost:8086/follow_db
spring.datasource.username=<database-username>
spring.datasource.password=<database-password>
```
4. Build the project using Maven:
```bash
cd follow-service
```
5. Run the application:
```bash
mvn spring-boot:run
```
## API Documentation
The Follow Service provides the following API endpoints:

- GET /follow/follows: Retrieves all follows.
- GET /follow/followed/{userid}: Retrieves the follows for a specific user.
- GET /follow/followers/{followedId}: Retrieves the followers for a specific user.
- POST /follow/addFollow: Adds a follow relationship between users.
- POST /follow/acceptRequest: Accepts a follow request.
- POST /follow/unFollow: Unfollows a user.
- GET /follow/requests/{userid}: Retrieves follow requests for a user.



