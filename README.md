# Dynamic_API_Security
A security application with JWT token to validated with MySQL DB.

# Technologies Used

    Spring Boot
    MySql database
    JWT Token based Authentication

   Application starts a Tomcat server on localhost port 8080. MySQL database has to be installed.

    Below are the test services to test the application
    http://localhost:8080/api/hello   
   
   
# Service Name

| HTTP  | METHODPATH | USAGE | Request | Response |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| POST | /api/register | To register the user | {"username": "sharath","password": "password"} | {"username": "sharath"} |
| POST | /api/authenticate | To retrive JWT token | {"username": "sharath","password": "password"} | {"token":"eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOMj"} |
| GET |	/api/hello    | Test with authentication |  - | Header : Bearer (token)xxxxx |
