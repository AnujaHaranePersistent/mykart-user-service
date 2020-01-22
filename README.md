# mykart-user-service


## Steps to Setup

### 1. Clone the application
```bash
https://github.com/AnujaHaranePersistent/mykart-user-service.git
```

### 2. Create Postgres database
```bash
create database mykart-data
```

### 3. Change postgres username and password as per your installation

``` bash
open src/main/resources/application.yml
```

change datasource.username and datasource.password as per your postgres installation 

### 4. Build and run the app using maven

```bash
mvn package
java -jar target/EmployeeDataService-0.0.1-SNAPSHOT.jar
```
Alternatively, you can run the app without packaging it using -

```bash
mvn spring-boot:run
```

The app will start running at http://localhost:5050.

# Explore Rest APIs

The app defines following CRUD APIs.

```bash
POST /login         -   to authenticate user and generate token

GET /api/v1/user/`         -   to get list of Users

POST /api/v1/user         -   to post user data to server

GET /api/v1/user/{user_id}     -   to get user with given identifier

PUT /api/v1/user/{user_id}     -   to update user with given identifier

DELETE /api/v1/user/{user_id}  -   to delete employee with given identifier

GET /manager/{id}          -   to get list of employees who reports to same manager
```

## To run Tests
 Type ``` mvn test ``` 
 from the root directory of the project to run the tests. 
 
 To view the jacaco generated report
 ``` bash
open D:\SpringRefrence\EmployeeDataService\target\site\jacoco\ident.html
```

 


