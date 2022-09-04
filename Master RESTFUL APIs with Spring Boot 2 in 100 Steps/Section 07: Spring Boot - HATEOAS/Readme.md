### Spring Boot HATEOAS
-   HATEOAS is an extra level upon REST.
-   It is used to present information about a REST API to a client without the need to bring up the API documentation.
-   It includes links in a returned response and client can use those API links to further communicate with the server.
-   Simplify the client by making the API discoverable.
-   This reduces the likelihood of client breaking due to changes to the service.

-   **spring-hateoas** provides two major wrapper classes. They are **EntityModel** and **CollectionModel**. Using these classes we can add the related links with few lines of code. Let’s see how I have done it.

### Step 58. Step-00: Introduction to Spring Boot - HATEOAS.md
-----------------------------------------------------------------------------
-   Step-00: Introduction
-----------------------------------------------------------------------------
-   Step-00: New GIT branch for HATEOAS
    git branch -vva
    git status
    git checkout -b 07-SpringBoot-HATEOAS
    git push --set-upstream origin 07-SpringBoot-HATEOAS
    git branch -a

### Step 59. Step-00: Create git branch for HATEOAS.md

### Step 60. Step-01: Add HATEOAS Dependency in pom.xml.md

-----------------------------------------------------------------------------
-   Step-01: Add Dependency in pom.xml
    - Add dependency in pom.xml (spring-boot-starter-hateoas)
    - Restart SpringBootApp (to reflect new dependency changes - new jar added)
    - POM.xml
    ```xml
        <dependency>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-starter-hateoas</artifactId>
        </dependency>
    ```        
-----------------------------------------------------------------------------

### Step 61. Step-02: Extend User and Order Entities with ResourceSupport.md
-----------------------------------------------------------------------------
-   Step-02: Extend both Entities to ResourceSupport
    - Entity Layer
        -  


### Step 62. Step-03: Create new User and Order Controllers for HATEOAS Implementation.md
-----------------------------------------------------------------------------
-   Step-03: Create new User and Order Controllers for HATEOAS Implementation
    - UserHateoasController
        - Create new UserHateoasController
        - Annotate with @RestController
        - Annotate with @RequestMapping(value = "/hateoas/users")
        - Annotate with @Validated
        - Autowire Repositories (UserRepository)
        - Copy Methods getUserById, getAllUsers from UserController    
    - OrderHateoasController
        - Create new OrderHateoasController 
        - Annotate with @RestController
        - Annotate with @RequestMapping(value = "/hateoas/users")
        - Autowire Repositories (UserRepository, OrderRepository)
        - Copy Methods getAllOrders from OrderController to OrderHateoasController  
    - Test with Postman
        - getUserById
            - GET /hateoas/users/{userid}
            - GET   http://localhost:8080/hateoas/users/101
            ```json
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
                ],
                "_links": {
                    "self": {
                        "href": "http://localhost:8080/hateoas/users/101"
                    },
                    "items": {
                        "href": "http://localhost:8080/hateoas/users/101/orders"
                        }
                    }
                }
            ```


        - getAllUsers
            - GET /hateoas/users
            - GET http://localhost:8080/hateoas/users
            ```json
            {
            "_embedded": {
                "userList": [
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
                        ],
                        "_links": {
                            "self": {
                                "href": "http://localhost:8080/hateoas/users/101"
                            },
                            "items": {
                                "href": "http://localhost:8080/hateoas/users/101/orders"
                            }
                        }
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
                                "orderDescription": "order21"
                            },
                            {
                                "orderId": 2005,
                                "orderDescription": "order22"
                            }
                        ],
                        "_links": {
                            "self": {
                                "href": "http://localhost:8080/hateoas/users/102"
                            },
                            "items": {
                                "href": "http://localhost:8080/hateoas/users/102/orders"
                            }
                        }
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
                                "orderDescription": "order31"
                            }
                        ],
                        "_links": {
                            "self": {
                                "href": "http://localhost:8080/hateoas/users/103"
                            },
                            "items": {
                                "href": "http://localhost:8080/hateoas/users/103/orders"
                            }
                        }
                    }
                            ]
                        },
                        "_links": {
                            "self": {
                                "href": "http://localhost:8080/hateoas/users"
                            }
                        }
                    }

            ```
        - getAllOrders  
            - GET /hateoas/users/{userid}/orders  
            - GET http://localhost:8080/hateoas/users/101/orders   
            ```json
            {
                "_embedded": {
                    "orderList": [
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
                },
                "_links": {
                    "self": {
                        "href": "http://localhost:8080/hateoas/users/101/orders"
                    }
                }
            }

            ```   
-----------------------------------------------------------------------------

### Step 63. Step-04: Implement self link in getUserById Method.md
-----------------------------------------------------------------------------
-   Step-04: Implement self link in getUserById Method 
    - UserHateoasController
        - getUserById - Self Linking        
        - Method: getUserById    
            - Extract UserId
            - Create Link using ControllerLinkBuilder
            - Add Link to Resource
            - Instead of User return type -  Resource<User> (Return Type changed to Resource) 
    - Test using Postman         
        - Method: getUserById
        - GET /hateoas/users/{userid}
-----------------------------------------------------------------------------


### Step 64. Step-05: Implement self and relationship links in getAllUsers Method.md

-----------------------------------------------------------------------------
-   Step-05: Implement self and relationship links in getAllUsers Method in UserHateoasController
    - 5(A) Self Link for each user in a for loop
        - UserHateoasController 
        - Method: getAllUsers    
        - HATEOAS: Implement self linking for each user
            - For loop
            - Extract User 
            - Create Link with ControllerLinkBuilder
            - Add link 
            - Change Return Type from List<User> to Resources<User>  
    - Test using Postman         
        - Method: getAllUsers
        - GET /hateoas/users
    - 5(B) Relation Ship Link with getAllOrders
        - UserHateoasController & OrderHateoasController
        - Method: getAllUsers    
        - HATEOAS: Implement relationship linking for getAllOrders
        - OrderHateoasController
            - Change getAllOrders method return type to "Resources<Order>" from List<Order>  
        - UserHateoasController
            - Create Link with ControllerLinkBuilder
            - Add Link
    - Test using Postman         
        - Method: getAllUsers
        - GET /hateoas/users  
    - 5(C) Self Link for getAllUsers   
        - UserHateoasController 
        - Method: getAllUsers    
        - HATEOAS: Implement self linking for getAllUsers Method
            - Create Link with ControllerLinkBuilder
            - Add link to Resource
    - Test using Postman         
        - Method: getAllUsers
        - GET /hateoas/users  
-----------------------------------------------------------------------------

### Step 65. Step06: GIT commit code, push to remote, merge to master.md
-----------------------------------------------------------------------------
Step-06: GIT commit code, push to remote, merge to master and push to remote 
git status
git add .
git commit -am "HATEOAS - First Commit"
git push
git checkout master
git merge 07-SpringBoot-HATEOAS
git branch -vva
-----------------------------------------------------------------------------
