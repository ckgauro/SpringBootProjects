## Validations
-   **Validating** user input is a very common & key requirement in today's world Spring Boot provides strong out of the box.
-   Spring Boot supports seamless integration with custom validators but the **de-facto** for performing validation is **Hibernate Validator**
    **(http://hibernate.org/validator/)**
-   **JSR 380**: JSR 380 is a specification of the Java API for bean validation, which ensures that properties of a bean meet specific criteria, using annotations such as **@NotNull, @Min, and @Max**
-   **@Valid** Annotation: When Spring boot finds an arugment annotated with **@Valid**, it automatically bootstraps the default JSR 380 implementation (Hibernate Validator) and validates the arugment. When the target arugment fails to pass the validation, Spring Boot throws a **MethodArgumentNotValidException**
-   Bean Validation 2.0 Specification - https://beanvalidation.org/2.0/

----------

## Commonly used - Validation Annotations

-   **@NotNull**: Validates that the annotated property value is not null
-   **@Size**: Validates that the annotated property value has a size between the attributes min and max
-   **@Min**: Validates that the annotated property has a value no smaller than the value attribute
-   **@Max**: Validates that the annotated property has a value no larger than the value attribute
-   **@Email**: Validates that the annoteated property is a valid email address
-   **@NotBlank**: Validate that the property is a valid email address
-   **@NotBlank**: Validate that the property is not null or whitespace
-   **@NotEmpty**: Validates that the property is not null or empty
-   **@AssertTrue**:    Validates that the annotated property value is true.

-----------

## Global Exception Handling

-   **@ControllerAdvice**
    -   Allows us to write global code that can be applied to a wide range of controllers.
    -   By default **@ControllerAdvice** annotation will be applicable to all classes that use **@Controller** which also applies for **@RestController**.

-   **@ExceptionHandler**
    -   Annotation for handling exception in specifiec handler class and/or handler methods.
    -   If used with controllers direclty, ew have the need to define it per controller but when used in combination with @ControolerAdvice it will be only in Global Exception Handler class but applicable to all controolers due to @ControllerAdvice.
-   **@RestControolerAdvice**
    -   @RestCollerAdvice is the combination of both **@ControllerAdvice** and **@ResponseBody**.
    -   We cna use the **@ControllerAdvice** annotation for handling exceptions in the RESTFUL Services but we need to add **@ResponseBody** separatley.

------------

## Usecase Combination

-   **@ControllerAdvice** & **ResponseEntityExceptionHandler** class
    -   MethodArguemntNotValidException
    -   HttpRequestMethodNotSupportException
-   **@ContollerAdvice** & **@ExceptionHandler**
    -   For pre-defined exceptions like **ConstraintViolationException**
    -   For custom exceptions like **UserNameNotFoundException**

-   **@RestControllerAdvice** & **@ExceptionHandler**
    -   For custom exceptions like **UserNameNotFoundException**
    -   For pre-defined exceptions like "**Exception.class**" (Applicable to all exceptions)        
### Step 40. Step-00: Introduction to Spring Boot - Validations & Global Exception Handling.md
---------------------------------------------------------------------------------------
Step-00: Introduction

### Step 41. Step-00: Create git branch for Validations & Global Exception Handling.md
---------------------------------------------------------------------------------------
Step-00: Create new git branch in local git repo and remote github repo
    - Verify we are in master branch    
        - git status
    - Create new branch
        - git checkout -b 05-Validations-GlobalExceptionHandler
    - Create new branch in remote github and setup upstream   
        - git push --set-upstream origin 05-Validations-GlobalExceptionHandler
    - Verify new branch in remote github & IDE GIT Perspective             
        - https://github.com/stacksimplify/springboot-buildingblocks             


### Step 42. Step-01: Implement Bean Validation - @Valid.md
---------------------------------------------------------------------------------------

-   Step-01: Implement Bean Validation
    - Entity Layer
        - Implement validations on User Entity
            - @NotEmpty(message = "Username is Mandatory field. Please provide username")
            - @Size(min=2, message="FirstName should have atleast 2 characters")            
    - Test using POSTMAN
         - Service: Create User Service
         - Request body
            - For firstname, give only 1 character  ("firstname": "K")
            - Send username as empty  ("username": "")
        - Verify Response on POSTMAN (JPA exception will be thrown)
    - Controller Layer
        - Enable Bean validation using @Valid
    - Test using POSTMAN
        - Service: Create User Service
        - Request body
            - For firstname, give only 1 character  ("firstname": "K")
            - Send username as empty  ("username": "")
        - Verify Response
            - HTTP Status 400 Bad request - with default response body 
            - MethodArgumentNotValidException resolved from logs   

        -   
        ```json
        {        
        "username": "",
        "firstname": "B",
        "lastname": "Reddy",
        "email": "kreddy@stacksimplify.com",
        "role": "admin",
        "ssn": "ssn10as45d"
        }
        ```
        - Result
        
        ```json
        {
            "timestamp": "2022-09-02T00:00:39.046+00:00",
            "status": 400,
            "error": "Bad Request",
            "message": "Validation failed for object='user'. Error count: 2",
            "errors": [
                {
                    "codes": [
                        "NotEmpty.user.username",
                        "NotEmpty.username",
                        "NotEmpty.java.lang.String",
                        "NotEmpty"
                    ],
                    "arguments": [
                        {
                            "codes": [
                                "user.username",
                                "username"
                            ],
                            "arguments": null,
                            "defaultMessage": "username",
                            "code": "username"
                        }
                    ],
                    "defaultMessage": "Username is Mandatory field. Please provide username",
                    "objectName": "user",
                    "field": "username",
                    "rejectedValue": "",
                    "bindingFailure": false,
                    "code": "NotEmpty"
                },
                {
                    "codes": [
                        "Size.user.firstname",
                        "Size.firstname",
                        "Size.java.lang.String",
                        "Size"
                    ],
                    "arguments": [
                        {
                            "codes": [
                                "user.firstname",
                                "firstname"
                            ],
                            "arguments": null,
                            "defaultMessage": "firstname",
                            "code": "firstname"
                        },
                        2147483647,
                        2
                    ],
                    "defaultMessage": "FirstName should have at least 2 characters",
                    "objectName": "user",
                    "field": "firstname",
                    "rejectedValue": "B",
                    "bindingFailure": false,
                    "code": "Size"
                }
            ],
            "path": "/users"
        }
        ```

--------------------------------------------------------------------------------------

### Step 43. Step-02: Implement custom Global Exception Handler - @ControllerAdvice.md

--------------------------------------------------------------------------------------
-   Step-02: Implement Custom Global Exception Handler - MethodArgumentNotValidException
    - Exception Layer - CustomErrorInfo class
        - Create a new class CustomErrorInfo                  
            - Define Variables date, message, errordetails
        - Add Fields Constructor
        - Add Getters                
    - Exception Layer - CustomGlobalExceptionHandler
        - Create a new class CustomGlobalExceptionHandler
        - extends ResponseEntityExceptionHandler
        - @ControllerAdvice
            - Global code that can be applied to a wide range of controllers.
        - Implement & Override handleMethodArgumentNotValid from ResponseEntityExceptionHandler
    - Test using POSTMAN
        - Method: POST 
        - Service: Create User Service
        - URI: http://locahost:8080/users
        - Request body
            - For firstname, give only 1 character  ("firstname": "K")
            - Send username as empty  ("username": "")
        - Verify Response
            - Custom Error Response
            - HTTP 400 Bad Request        

        -   JSON
        ```JSON
         {        
        "username": "",
        "firstname": "B",
        "lastname": "Reddy",
        "email": "kreddy@stacksimplify.com",
        "role": "admin",
        "ssn": "ssn10as45d"
        }
            
        ```
        -   Result
        ```json
        {
        "timestamp": "2022-09-02T18:13:10.404+00:00",
        "message": "Validation failed for argument [0] in public org.springframework.http.ResponseEntity<java.lang.Void> com.gauro.restservices.springbootbuildingblocks.restservices.controllers.UserController.createUser(com.gauro.restservices.springbootbuildingblocks.restservices.entities.User,org.springframework.web.util.UriComponentsBuilder) with 2 errors: [Field error in object 'user' on field 'username': rejected value []; codes [NotEmpty.user.username,NotEmpty.username,NotEmpty.java.lang.String,NotEmpty]; arguments [org.springframework.context.support.DefaultMessageSourceResolvable: codes [user.username,username]; arguments []; default message [username]]; default message [Username is Mandatory field. Please provide username]] [Field error in object 'user' on field 'firstname': rejected value [B]; codes [Size.user.firstname,Size.firstname,Size.java.lang.String,Size]; arguments [org.springframework.context.support.DefaultMessageSourceResolvable: codes [user.firstname,firstname]; arguments []; default message [firstname],2147483647,2]; default message [FirstName should have at least 2 characters]] ",
        "errorDetails": "From MethodArgumentNotValid Exception in GEH"
        }
        
        ```                   

---------------------------------------------------------------------------------------



### Step 44. Step-03: Implement HttpRequestMethodNotSupportedException in GEH.md

---------------------------------------------------------------------------------------

-   Steo-03: Implement "HttpRequestMethodNotSupportedException" in Custom Global Exception Handler
    - Test using POSTMAN
        - Provide PATCH method for create user
        - Verify response code and body   
    - Exception Layer -  CustomGlobalExceptionHandler
        - Implement & Override handleHttpRequestMethodNotSupported from ResponseEntityExceptionHandler 
    - Test using POSTMAN
        - Provide PATCH method for create user
        - Verify response code and body  
        - URI: http://locahost:8080/users
        - Verify Response
            - Custom Error Response
            - HTTP 400 Bad Request           
    -   JSON INput
    ```json
     {        
        "username": "",
        "firstname": "B",
        "lastname": "Reddy",
        "email": "kreddy@stacksimplify.com",
        "role": "admin",
        "ssn": "ssn10as45d"
    }

    -   Result
    ```json
    {
    "timestamp": "2022-09-02T18:21:02.924+00:00",
    "message": "Request method 'PATCH' not supported",
    "errorDetails": "From HttpRequestMethodNotSupportedException in GEH -Method Not Allowed"
    }


    ```



---------------------------------------------------------------------------------------



### Step 45. Step-04: Implement UserNameNotFoundException in GEH - @ExceptionHandler.md

---------------------------------------------------------------------------------------
-   Step-04: Implement ExceptionHandler for custom exception like "UserNameNotFoundException"
    - Exception Layer
        - Create a new class "UserNameNotFoundException" 
            - extends Exception
            - Generate constructor from Super class
    - Controller Layer
        - For getUserbyUsername Method, Throw UserNameNotFoundException if that user doesnt exists in Repository.
    - Test using POSTMAN
        - Method: GET
        - URI: http://localhost:8080/users/byusername/abcd
        - Verify default spring Exception (Response code HTTP 500)
    - Exception Layer -  CustomGlobalExceptionHandler
        - Create handleUserNameNotFoundException method
        - Annotate it with @ExceptionHandler
    - Test using POSTMAN
        - Method: GET
        - URI: http://localhost:8080/users/byusername/abcd
        - Verify the Response Body and HTTP Status Code 404  
    - Result

    ```json
    {
    "timestamp": "2022-09-02T18:31:27.374+00:00",
    "message": "UserName :'abcd' not found in useer Repository",
    "errorDetails": "uri=/users/byusername/abcd"
    }
    
    ```            

---------------------------------------------------------------------------------------


### Step 46. Step-05: Path Variable Validation & ConstraintViolationException in GEH.md

---------------------------------------------------------------------------------------
-   Step-05: Path Variables Validation & Handling ConstraintViolationException using CustomGlobalExceptionHandler
    - Contoller Layer
        - getUserById method: Add @Min(1) for Path Variable
        - Add @Validated annotation to UserController class
    - Test using POSTMAN
        - Method: GET
        - URI: http://localhost:8080/users/0
        - Verify default spring Exception (Response code HTTP 500)
    - Exception Layer -  CustomGlobalExceptionHandler
        - Create handleConstraintViolationException class 
        - Annotate it with @ExceptionHandler
    - Test using POSTMAN
        - Method: GET
        - URI: http://localhost:8080/users/0
        - Verify the Response Body and HTTP Status Code - 400   
        -   Result
        ```json
        {
            "timestamp": "2022-09-02T22:49:29.184+00:00",
            "message": "getUserId.id: must be greater than or equal to 1",
            "errorDetails": "uri=/users/0"
        }
        ```
    - Test using POSTMAN
        - Method: GET
        - URI: http://localhost:8080/users/1000
        -   Result
        ```json
            {
        "timestamp": "2022-09-02T22:50:18.436+00:00",
        "status": 404,
        "error": "Not Found",
        "message": "User not found in user Repository",
        "path": "/users/1000"
        }
    ```
---------------------------------------------------------------------------------------


### Step 47. Step-06: Implement Global Exception Handling using @RestControllerAdvice.md

---------------------------------------------------------------------------------------
-   Step-06: Implement Global Exception Handling using RestControllerAdvice
    - Exception Layer - CustomGlobalExceptionHandler
        - Comment @ControllerAdvice
        - Test to ensure controller advice is not in action for getUserByUsername
    - Exception Layer 
        - Create new class GlobalRestControllerAdviceExceptionHandler
        - Annotate with @RestControllerAdvice
        - Handle UserNameNotFoundException        
            - Create a mehtod notFound 
            - Annotate it with @ExceptionHandler
            - Annotate it with @ResponseStatus - 404
    - Test using POSTMAN
        - Method: GET
        - URI: http://localhost:8080/users/byusername/abcd12
        - Verify the Response Body and HTTP Status Code  - 404  
        -   RESULT
        ```JSON
        {
            "timestamp": "2022-09-02T23:34:00.707+00:00",
            "message": "UserName :'abcd12' not found in useer Repository",
            "errorDetails": "From @RestController Not Found"
        }
    ```



### Step 48. Step-07: Switching between @ControllerAdvice and @RestControllerAdvice.md

---------------------------------------------------------------------------------------
Step-07: Note about switching between **@ControllerAdvice and @RestControllerAdvice**

Step-08: GIT Commit, Push, Merge to Master and Push

