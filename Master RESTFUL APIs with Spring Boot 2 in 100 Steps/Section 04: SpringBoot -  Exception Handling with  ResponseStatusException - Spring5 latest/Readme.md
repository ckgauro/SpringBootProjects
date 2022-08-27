 
### Step 31. Step-00: Introduction to Exception Handling using ResponseStatusException.md

-   #### Exception Handling and Response Status Codes
-   ResponseStatusException Class
    -   Spring5 introduces the **ResponseStatusException** class which is a fast way for basic error handling in our RESTful API's.
    -   It is an **alternative** to **@ResponseStatus** and is the base class for exceptions used for applying status code to an  **HTTP Response**
    -   We can create an instance of it providing and **HttpStatus** and optionally a **reason** and a **cause**.
    -   It's a **RuntimeException**.
    -   ResponseStatusException constructor arguments
        -   **status** - an HTTP Status set to HTTP response
        -   **reason** - a message explaining the exception set to that particular HTTP response.
        -   **cause** - a Throwable cause of the ResponseStatusException
    -   **Benefits**
        -   We can implement it quite **fast**
        -   There is no specific need for creating **custom exception classess**, unless we have a need becasue we can define HTTP Response Status code and Error message at a time.
        -   As we are creating exceptions programmatically, we will have **more control** over exception handling
    -   **Downside**
        -   **Code Duplication** As we are defining them programmatically, ew find ourselves replicatiing code in multiple controllers.
        -   **Global Exception Handling**: This approach will not look like a global approach like **@ControllerAdvice**. Its difficult to enforce applicaiton-wide conventions.
    -   **Combine Approaches**
        - We can implement **@ControllerAdvice** globally and **ResponseStatueExceptions** locally as anbd when required.

#### Creating Steps
-   Step-00: Create git branch - local & remote.md
-   Step 33. Step-01: Implement ResponseStatusException handling for getUserById.md
-   Step 34. Step-02: Implement ResponseStatusException for updateUserById RESTful Service.md
-   Step 35. Step-03: Implement ResponseStatusException for deleteUserById RESTful Service.md
-   Step 36. Step-04: Implement ResponseStatusException for createUser RESTful Service.md
-   Step-05: Implement HTTP Status code & Location Header for createUser Service.md

### Step 32. Step-00: Create git branch - local & remote.md


---------------------------------------------------------------------------------------
Step-00: Create new git branch in local git repo and remote github repo
    - Verify we are in master branch    
        - git status
    - Create new branch
        - git checkout -b 04-ExceptionHandling-ResponseStatusCodes
    - Create new branch in remote github and setup upstream   
        - git push --set-upstream origin 04-ExceptionHandling-ResponseStatusCodes
    - Verify new branch in remote github & IDE GIT Perspective             
        - https://github.com/stacksimplify/springboot-buildingblocks             
        
-   $git status


### Step 33. Step-01: Implement ResponseStatusException handling for getUserById.md

----------------------------------------------------------------------------------------
Step-01: Implement "ResponseStatusException" for getUserById
    - Custom Exceptions Layer: 
        - Create "UserNotFoundException" which extends Exception
    - Service Layer:
        - Update the getUserById method with throws Exception
        - Check for user and if not exists throw exception. 
    - Controller Layer: 
        - Update the getUserById method with try catch block.
        - In catch block, implement "ResponseStatusException".
    - Test using postman. 
        - Method: GET 
        - URI: http://localhost:8080/users/1001
    - Remove Trace in Exception.
        - When using DevTools, "server.error.include-stacktrace" will be set to always
        - change to never or on-trace-param
    - Verify the response again.      
        - Exception Message
        - HTTP Status Code           


### Step 34. Step-02: Implement ResponseStatusException for updateUserById RESTful Service.md

### Step 35. Step-03: Implement ResponseStatusException for deleteUserById RESTful Service.md
### Step 36. Step-04: Implement ResponseStatusException for createUser RESTful Service.md

### Step 37. Step-05: Implement HTTP Status code & Location Header for createUser Service.md

### Step 38. Step-06: GIT Commit, Push, Merge to Master and Push.md
