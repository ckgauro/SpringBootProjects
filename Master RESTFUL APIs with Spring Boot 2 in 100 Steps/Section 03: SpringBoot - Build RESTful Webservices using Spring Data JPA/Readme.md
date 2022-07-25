 
### Step 14. Step-00: Introduction to Build RESTful APIs with JPA .md
Step 01: **Usecase** Introduction
Step-02: Verify pom.xml for all Dependencies
Step-03: Update application.properties required for JPA based RESTful Services
Step-04-01: Create User Entity - Understand @Entity Annotation
Step-04-02: Create User Entity - Understand @Table Annotation 
Step-04-03: Create User Entity - Define Variables, Getters & Setters
Step-05: Understand and Implement changes related to H2 Database 
Step-06: Create User Repository - @Repository 
Step-07: Implement getAllUsers RESTful Service - @Service, @RestController 
Step-08: Test getAllUsers RESTful Service - Using REST Client POSTMAN 
Step-09: Implement createUser RESTful Service - @PostMapping 
Step-10: Implement getUserById RESTful Service - @GetMapping 
Step-11: Implement updateUserById RESTful service - @PutMapping 
Step-12: Implement deleteUserById RESTful Service - @DeleteMapping 
Step-13: Implement getUserByUsername RESTful Service - @GetMapping 
Step-14: GIT Commit, Push, Merge to Master and Push 


### Step 15. Step-01: Usecase Introduction .md
Step-01: Usecase Introduction - User Management Service
   - Create User  - POST - /users
   - Get All Users - GET - /users
   - Get User By Id - GET - /users/{id}
   - Update User By Id - PUT - /users/{id}
   - Delete User By Id - DELETE - /users/{id}
   - Get User By username - GET - /users/byusername/{username}   
### Step 16. Step-02: Verify pom.xml for all Dependencies .md

Step-02: Verify pom.xml for all Dependencies
   - Mandatory
       - SpringBoot Starter Web    
       - Spring Boot Data JPA
       - H2 Database
   - Optional
        - Spring Boot DevTools    
   - Create GIT Branch
      - Create GIT branch name "03-JPA-UsermgmtService-Base"    

### Step 17. Step-03: Update application.properties required for JPA based RESTful Services .md  --Done

Create GIT branch name "03-JPA-UsermgmtService-Base"  

application.properties
```properties
spring.jpa.show-sql=true
spring.h2.console.enabled=true
```

### Step 18. Step-04-01: Create User Entity - Understand @Entity Annotation .md -- Done

Step-04: Entity
    - Fields or Variables (id, username, firstname, lastname, email, role, ssn)
    - @Entity
    - @Table
    - @Id
    - GeneratedValue
    - @Column (name, length, nullable, unique)
    - No Arg Constructor    
    - Fields Constructor   
    - To String (Optional for bean logging)   

https://github.com/stacksimplify/springboot-buildingblocks/blob/03-JPA-UserMgmtService-Base/src/main/java/com/stacksimplify/restservices/entities/User.java

### Step 19. Step-04-02: Create User Entity - Understand @Table Annotation .md


https://github.com/stacksimplify/springboot-buildingblocks/blob/03-JPA-UserMgmtService-Base/src/main/java/com/stacksimplify/restservices/entities/User.java
    
### Step 20. Step-04-03: Create User Entity - Define Variables, Getters & Setters .md

https://github.com/stacksimplify/springboot-buildingblocks/blob/03-JPA-UserMgmtService-Base/src/main/java/com/stacksimplify/restservices/entities/User.java
### Step 21. Step-05: Understand and Implement changes related to H2 Database .md
      
Step-05: H2 Database
- In Memory Database (data will be lost when we restart JVM or when JVM reloads)
- Prepopulate DB during runtime with data
- Create data.sql in src/main/resources
- Note: Columns will be created in Alphabetical order in DB except primary Key Id
- Note: So insert statement values should be in alphabetical order as 
displayed in H2 DB or write insert statements with column names for User table too. 
- H2 Console: http://localhost:8080/h2-console
- JDBC URL: jdbc:h2:mem:testdb

H2 DB Records 
insert into user values(101, 'kreddy@stacksimplify.com', 'Kalyan', 'Reddy', 'admin', 'ssn101', 'kreddy');
insert into user values(102, 'gwiser@stacksimplify.com', 'Greg', 'Wiser', 'admin', 'ssn102', 'gwiser');
insert into user values(103, 'dmark@stacksimplify.com', 'David', 'Mark', 'admin', 'ssn103', 'dmark');          

https://github.com/stacksimplify/springboot-buildingblocks/blob/03-JPA-UserMgmtService-Base/src/main/resources/data.sql

localhost:8080/h2-console
### Step 22. Step-06: Create User Repository - @Repository .md
     



Step-06: Repository
   - Create a Interface
   - extends JpaRepository
   - @Repository     

https://github.com/stacksimplify/springboot-buildingblocks/blob/03-JPA-UserMgmtService-Base/src/main/java/com/stacksimplify/restservices/repositories/UserRepository.java

### Step 23. Step-07: Implement getAllUsers RESTful Service - @Service, @RestController .md
   
Step-07: Implement getAllUsers Method 
    - Service: 
        - Create a UserService class 
        - Annotate it with @Service
        - @Autowired (Autowire UserRepository)
        - Create getAllUsers Method
    - Controller: 
        - Create a UserController class
        - Annotate it with @RestController
        - @Autowired (Autowire UserService)
        - Create @GetMapping for getAllUsersMethod   

### Step 24. Step-08: Test getAllUsers RESTful Service - Using REST Client POSTMAN .md
      
Step-08: Test using REST Client - POSTMAN
    - Download & Install POSTMAN - https://www.getpostman.com/
    - Create Collection "SpringBoot-BuildingBlocks"
    - Create a request for getAllUsers
        - Method: GET
        - URI: http://localhost:8080/users
    - Test and Verify getAllUsers RESTful service.     

Test:
-  localhost:8080/users/1    

### Step 25. Step-09: Implement createUser RESTful Service - @PostMapping .md
     
----------------------------------------------------------------------------------------------
Step-09: Implement createUser Method in Service & Controller Layers
    - Service Layer: 
        - Implement createUser Method
    - Controller Layer
        - Implement createUser Method
            - @RequestBody Annotation
        - Add @PostMapping Annotation to createUser Method
    - POSTMAN: Verify the createUser RESTful service  in postman REST client
        -  Create a request for createUser  
            -  Body (select raw)
            - Content Type: JSON (application/json)
            - Method: POST
        -  Test using postman   


Test using POSTMAN:
-  POST : localhost:8080/users/1         
   {
     "username": "chandra",
    "firstName": "gauro",
    "lastName": "Reddy",
    "email": "kreddy@stacksimplify.com",
    "role": "admin",
    "ssn": "ssn101"
   }

-     

### Step 26. Step-10: Implement getUserById RESTful Service - @GetMapping .md 
------------------------------------------------
Step-10: Implement getUserById Method in Service and Controller Layers
    - Service Layer: 
        - Create getUserById Method
        - Discuss about return type Optional Object
    - Controller Layer: 
        - Create getUserById Method and apply Optional return type
        - @PathVariable Annotation
        - Annotate @GetMapping for getUserById Method 
        - URI: /users/{id}
    - POSTMAN: Create & Verify the getUserById RESTful Service in postman REST client
        - Method: GET 
        - URL: http://localhost:8080/users/{id}
        - URL: http://localhost:8080/users/103


Test using POSTMAN:
-  Get : localhost:8080/users/1         
   
-  GET: localhost:8080/users
### Step 27. Step-11: Implement updateUserById RESTful service - @PutMapping .md
----------------------------------------------------------------------------------------------    
Step-11: Implement updateUserById Method in Service and Controller layers
    - Service Layer: 
        - Create updateUserById Method
        - Inputs (User, Id)
    - Controller Layer: 
        - Create updateUserById Method
        - @PathVariable
        - @RequestBody
        - Annotate @PutMapping for updateUserById Method
    - POSTMAN: Verify updateUserById RESTful service in postman REST client
        -  Create a request for updateUserById  
            - Body (select raw)
            - Content Type: JSON (application/json)
            - Method: PUT
            - In URI: /users/{id}
        -  Test using postman   

Test using POSTMAN:
-  PUT : localhost:8080/users/1         
   {
     "username": "chandra",
    "firstName": "gauro",
    "lastName": "Reddy",
    "email": "kreddy@stacksimplify.com",
    "role": "admin",
    "ssn": "ssn101"
   }
-  GET: localhost:8080/users
### Step 28. Step-12: Implement deleteUserById RESTful Service - @DeleteMapping .md
  Step-12: Implement deleteUserById Method in Service and Controller Layers
    - Service Layer: 
        - Create deleteUserById Method
        - Verify user exists and then delete it
    - Controller Layer: 
        - Create deleteUserById Method
        - @PathVariable Annotation
        - Annotate @DeleteMapping for deleteUserById Method
    - POSTMAN: Verify deleteUserById Service in postman REST client
        - Method: DELETE
        - URL: http://localhost:8080/users/{id}
        - URL: http://localhost:8080/users/103


Test using POSTMAN:
-  Delete : localhost:8080/users/1         
  
-  GET: localhost:8080/users
### Step 29. Step-13: Implement getUserByUsername RESTful Service - @GetMapping .md
Step-13: Implement getUserByUsername Method in Repository, Service & Controller Layers
    - Repository Layer: 
        - Define "findByUsername" in UserRepository Interface
    - Service Layer: 
        - Create getUserByUsername Method 
        - Input as username (String)
    - Controller Layer: 
        - Create getUserByUsername Method
        - @PathVariable Annotation
        - Annotate @GetMapping for getUserByUsername Method
        - URI: /users/byusername/{username}
    - POSTMAN: Create & Verify the getUserByUsername RESTful Service in postman REST client
        - Method: GET 
        - URL: http://localhost:8080/users/byusername/{username}
        - URL: http://localhost:8080/users/byusername/kreddy


      
Test using POSTMAN:
-  GET : http://localhost:8080/users/byusername/kreddy       
   
-  GET: localhost:8080/users 
### Step 30. Step-14: GIT Commit, Push, Merge to Master and Push .md

----------------------------------------------------------------------------------------------
Step-14: GIT Commit & Merge to Master & Push
    - Branch: 03-JPA-UserMgmtService-Base
        - Commit & Push 
    - Branch: Master
        - Merge from branch 03-JPA-UserMgmtService-Base
        - Commit & Push
    -  Verify in github        
