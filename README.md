# JournalNest

## Overview
It is an Platform where users can post there Journal.


## Features
- Spring Boot framework
- MongoDB integration
- RESTful APIs
- CRUD operations

## Prerequisites
Ensure you have the following installed:
- Java 17 or later
- Maven 3.6+
- MongoDB (local or cloud instance)

## Setup & Configuration
### 1. Clone the Repository
```sh
 git clone <repository-url>
 cd <project-directory>
```

### 2. Configure MongoDB Connection
Modify `src/main/resources/application.properties` or `application.yml`:

#### For Local MongoDB
```properties
spring.data.mongodb.uri=mongodb://localhost:27017/yourDatabaseName
```

#### For MongoDB Atlas
```properties
spring.data.mongodb.uri=mongodb+srv://username:password@cluster.mongodb.net/yourDatabaseName?retryWrites=true&w=majority
```

### 3. Build & Run the Application
Use Maven to build and run the application:
```sh
mvn clean install
mvn spring-boot:run
```

### 4. Access the API
Once the application is running, you can access the API at:
```
http://localhost:8080/
```

## API Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/resource` | Get all records |
| POST | `/api/resource` | Create a new record |
| PUT | `/api/resource/{id}` | Update a record |
| DELETE | `/api/resource/{id}` | Delete a record |

## Troubleshooting
1. **Invalid MongoDB Connection String:** Ensure your connection string starts with `mongodb://` or `mongodb+srv://`.
2. **MongoDB Not Running:** Start MongoDB using `mongod`.
3. **Incorrect Credentials:** Double-check username and password for MongoDB Atlas.

## License
This project is licensed under the MIT License.

## Author
[Your Name]


