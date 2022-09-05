
[video 71, 72, 75]

### Static Filtering

-   Static Filtering
    -   @JsonIgnore will be applied at field level in a model class (Entity)
    -   @JsonIgnoreProperties will be applied class level in a model class and we cna define list of fields that can be ignored
    -   Simply hides the field from the Jackson parser
    -   Create or update request will fail after applying these annotations (POST, PUT)
### Step 71. Step-01: Implement Static Filtering using @JsonIgnore and @JsonIgnoreProperties.md
-   Step-01: New GIT branch (usign IDE)
    - git Branch name: 09-01-SpringBoot-Filtering-JsonIgnore
    - Create new local branch
-   Step-02: Static Filtering  
    - Entity Layer
        - @JsonIgnore - Apply to SSN field
        - Test
        -   GET http://localhost:8080/users/101
        ```json
        {
        "id": 101,
        "username": "kreddy",
        "firstname": "Kalyan",
        "lastname": "Reddy",
        "email": "kreddy@stacksimplify.com",
        "role": "admin",
        "orders": [
            {
                "orderId": 2001,
                "orderDescription": "order11",
                "links": []
            },
            {
                "orderId": 2002,
                "orderDescription": "order12",
                "links": []
            },
            {
                "orderId": 2003,
                "orderDescription": "order13",
                "links": []
            }
        ],
        "links": []
        }

        ```
        -   POST http://localhost:8080/users
        -   JSON
        ```json
         {        
        "username": "Chandra",
        "firstname": "sdfB",
        "lastname": "Reddy",
        "email": "kreddy@stacksimplify.com",
        "role": "admin",
        "ssn": "ssn10as45d"
        }
        ```
        -   Result throws error due to @JSONIgnore
        ```json
        {
        "timestamp": "2022-09-04T17:28:41.171+00:00",
        "status": 500,
        "error": "Internal Server Error",
        "message": "could not execute statement; SQL [n/a]; constraint [null]; nested exception is org.hibernate.exception.ConstraintViolationException: could not execute statement",
        "path": "/users"
        }
        ```



        - @JsonIgnoreProperties - Apply to firstname and lastname
        - Test
        -   GET http://localhost:8080/users/101
        - result
        ```json
        {
        "id": 101,
        "username": "kreddy",
        "email": "kreddy@stacksimplify.com",
        "role": "admin",
        "orders": [
            {
                "orderId": 2001,
                "orderDescription": "order11",
                "links": []
            },
            {
                "orderId": 2002,
                "orderDescription": "order12",
                "links": []
            },
            {
                "orderId": 2003,
                "orderDescription": "order13",
                "links": []
            }
        ],
        "links": []
        }

        ```    
### Step 72. Step-02: Implement Dynamic Filtering using MappingJacksonValue.md

#### Dynamic Filtering
-   We are going to use **MappingJacksonValue** to implement dynamic filtering
-   @JsonFilter applied at Model class with filtername.
-   Rest all logic related to filtering will be defined in service or controller layer


-   Step-01: New GIT branch (usign IDE)
    - git Branch name: 09-02-SpringBoot-Filtering-MappingJacksonValue
    - Create new local branch
-----------------------------------------------------------------------------
-   Step-02: Dynamic Filtering using MappingJacksonValue class
    - Controller Layer
        - Create a new UserMappingJacksonController
        - Copy getUserById methods.
    - UserMappingJacksonController
        - Implement filtering with static hashset 
        - Test it
        - Convert the same to a dynamic filtering by using @RequestParam
        - Test it   

        -   Test
        -   POSTMAN
        -   GET http://localhost:8080/jacksonfilter/users/101
        -   Result
        - 
        ```json
        {
            "username": "kreddy",
            "ssn": "ssn101",
            "orders": [
                {
                    "orderId": 2001,
                    "orderDescription": "order11"
                },
                {
                    "orderId": 2002,
                    "orderDescription": "order12"
                },
                {
                    "orderId": 2003,
                    "orderDescription": "order13"
                }
            ]
        }
        ```

        -   Test
        -   POSTMAN
        -   GET http://localhost:8080/jacksonfilter/users/params/101
        -  POSTMAN Parameters
            - Fields: userid,username,ssn,firstname,orders
        -   Result
        - 
        ```json
        {
            "username": "kreddy",
            "firstname": "Kalyan",
            "ssn": "ssn101",
            "orders": [
                {
                    "orderId": 2001,
                    "orderDescription": "order11"
                },
                {
                    "orderId": 2002,
                    "orderDescription": "order12"
                },
                {
                    "orderId": 2003,
                    "orderDescription": "order13"
                }
            ]
        }
        ```


### Step 73. Step-03: Implement Dynamic Filtering with MappingJacksonValue & @RequestParam.md
-----------------------------------------------------------------------------
-   Step-00: Introduction
-----------------------------------------------------------------------------
-   Step-01: New GIT branch (usign IDE)
    - git Branch name: 09-02-SpringBoot-Filtering-MappingJacksonValue
    - Create new local branch
-----------------------------------------------------------------------------
-   Step-02: Dynamic Filtering using MappingJacksonValue class
    - Controller Layer
        - Create a new UserMappingJacksonController
        - Copy getUserById methods.
    - UserMappingJacksonController
        - Implement filtering with static hashset 
        - Test it
        - Convert the same to a dynamic filtering by using @RequestParam
        - Test it      
 -----------------------------------------------------------------------------
-   Step-03: Commit Code (using IDE)
    - Commit code
    - Push branch to Remote repo
-----------------------------------------------------------------------------


### Step 74. Step-04: Dynamic Filtering - git Commit and Push code.md

### Step 75. Step-05: Introduction to Filtering using @JsonView.md
   

### Step 76. Step-06: Implement Filtering using @JsonView.md

#### @JsonView
-   @JsonView is used to customize views.
-   Applied at field level in a model class to categorize which field belongs to which view.
-   Applied at service level in a controller, so that for that respective REST service, view defined in @JsonView will be applicable.
-   Will be very useful if we have a single entity or model which need to be provided with different views to different category of clients.

-----------------------------------------------------------------------------
-   Step-00: Introduction
-----------------------------------------------------------------------------
-   Step-01: New GIT branch (usign IDE)
    - git Branch name: 09-03-SpringBoot-Filtering-JsonView
    - Create new local branch
-----------------------------------------------------------------------------
-   Step-02: @JsonView
    - Entity Layer 
        - Create a class named Views
            - Create two static classes in View (External, Internal)
        - Annotate fields in User Entity with @JsonView 
        - Decide which fields should be external and internal and annotate accordingly.             
    - Controller Layer
        - Create new controller named "UserJsonViewController"
        - Copy getUserById method from UserController and create two methods
            - External getUserById
                - GET /jsonview/users/external/101
                - Annotate with @JsonView(Views.External.class)
                -  Test it using Postman
                -   http://localhost:8080/jsonview/users/external/101
                - Result
                ```json
                    {
                        "id": 101,
                        "username": "kreddy",
                        "firstname": "Kalyan",
                        "lastname": "Reddy",
                        "email": "kreddy@stacksimplify.com"
                    }
                ```
            - Internal getUserById2
                - GET /jsonview/users/internal/101
                - Annotate with @JsonView(Views.Internal.class)
                -  Test it using Postman  
                - Result
                ```json
                [
                    {
                        "id": 1,
                        "username": "Chandra",
                        "firstname": "sdfB",
                        "lastname": "Reddy",
                        "email": "kreddy@stacksimplify.com",
                        "role": "admin",
                        "ssn": "ssn10as45d",
                        "orders": [],
                        "links": []
                    },
                    {
                        "id": 101,
                        "username": "kreddy",
                        "firstname": "Kalyan",
                        "lastname": "Reddy",
                        "email": "kreddy@stacksimplify.com",
                        "role": "admin",
                        "ssn": "ssn101",
                        "orders": [
                            {
                                "orderId": 2001,
                                "orderDescription": "order11",
                                "links": []
                            },
                            {
                                "orderId": 2002,
                                "orderDescription": "order12",
                                "links": []
                            },
                            {
                                "orderId": 2003,
                                "orderDescription": "order13",
                                "links": []
                            }
                        ],
                        "links": []
                    },
                    {
                        "id": 102,
                        "username": "gwiser",
                        "firstname": "Greg",
                        "lastname": "Wiser",
                        "email": "gwiser@stacksimplify.com",
                        "role": "admin",
                        "ssn": "ssn102",
                        "orders": [
                            {
                                "orderId": 2004,
                                "orderDescription": "order21",
                                "links": []
                            },
                            {
                                "orderId": 2005,
                                "orderDescription": "order22",
                                "links": []
                            }
                        ],
                        "links": []
                    },
                    {
                        "id": 103,
                        "username": "dmark",
                        "firstname": "David",
                        "lastname": "Mark",
                        "email": "dmark@stacksimplify.com",
                        "role": "admin",
                        "ssn": "ssn103",
                        "orders": [
                            {
                                "orderId": 2006,
                                "orderDescription": "order31",
                                "links": []
                            }
                        ],
                        "links": []
                    }
                ]

                ``` 


Step-03: Commit Code (using IDE)
    - Commit code
    - Push branch to Remote repo
-----------------------------------------------------------------------------



