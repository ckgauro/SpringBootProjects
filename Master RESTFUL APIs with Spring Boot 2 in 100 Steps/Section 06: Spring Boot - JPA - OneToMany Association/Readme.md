 
### Step 49. Step-00: Need for JPA OneToMany for HATEOAS.md
-----------------------------------------------------------------------------
-   Step-00: Usecase Introduction
    - Get All orders of a User 
        - Method Name: getAllOrders    
        - GET /users/{userid}/orders
    - Create an order for a user
        - Method Name: createOrder
        - GET /users/{userid}/orders
    - Get order details using orderid and userid
        - Method Name: getOrderByOrderId
        - GET /users/{userid}/orders/{orderid}        
-----------------------------------------------------------------------------

### Step 50. Step-00: Introduction to JPA OneToMany Association.md
### Step 51. Step-01: Create git branch for JPA OneToMany Association.md
-   Step-01: Create GIT branch for JPA @OneToMany Association
    git branch -vva
    git status
    git checkout -b 06-SpringBoot-JPA-OneToMany
    git push --set-upstream origin 06-SpringBoot-JPA-OneToMany
    git branch -a

-----------------------------------------------------------------------------

### Step 52. Step-02: Create Order Entity and @ManyToOne Association.md

-----------------------------------------------------------------------------
-   Step-02: Create Order entity and ManyToOne Mapping
    - Entity Layer
        - Create Order Entity
        - Annotate with @Table(name = "orders")
        - Add User variable
        - Add @ManyToOne Mapping
        - Add Fetch Type as lazy
        - Add @JsonIgnore
        - Add Getters and setters
        - Add NoArgument Constructor
 
-----------------------------------------------------------------------------


### Step 53. Step-03: Update User entity with @OneToMany Association.md
-   Step-03: Update User entity with @OneToMany association
    - Add orders variable
    - Add @OneToMany Mapping
    - Add MappedBy to user variable in Order Entity
    - Add getters and setters for "orders"
    - src/main/resources
        - update data.sql
Option#1: Verify Column and create insert query       
insert into orders values( 2001, 'order11', 101);        
insert into orders values( 2002, 'order12', 101);
insert into orders values( 2003, 'order13', 101);
insert into orders values( 2004, 'order21', 102);
insert into orders values( 2005, 'order22', 102);
insert into orders values( 2006, 'order31', 103);
Option#2: Verify Foreign Key name in DB before creating below insert queries
insert into orders (orderid, orderdescription, user_user_id) values( 2001, 'order11', 101);
insert into orders (orderid, orderdescription, user_user_id) values( 2002, 'order12', 101);
insert into orders (orderid, orderdescription, user_user_id) values( 2003, 'order13', 101);
insert into orders (orderid, orderdescription, user_user_id) values( 2004, 'order21', 102);
insert into orders (orderid, orderdescription, user_user_id) values( 2005, 'order22', 102);
insert into orders (orderid, orderdescription, user_user_id) values( 2006, 'order31', 103);

    - Test using Postman
        - Test#1: getAllUsers
            - GET /users
        - Test#2: getUserById 
            - GET /users/101  
-----------------------------------------------------------------------------

### Step 54. Step-04: Implement getAllOrders RESTful Service.md
-----------------------------------------------------------------------------
-   Step-04: Implement "getAllOrders" method in OrderController 
    - Controller Layer: UserController
        - Add @RequestMapping at class level and add "/users" context at class level
        - Remove "/users" at method level for all User related methods. 
        - This will help us when creating self links in HATEOAS section.
    - Controller Layer: OrderController
        - Annotate with @RestController
        - Annotate with @RequestMapping
        - Method: getAllOrders
        - GET /users/{userid}/orders
    - Test using Postman
        - Test#1: getAllOrders
            - GET /users/101/orders
            -   Result
            ```json
                    [
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
                
            ```
        - Test#2: getAllUsers
            - GET /users 
            -   Result
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
            ]
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
                    ]
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
                    ]
                }
            ]
            ```                          
        - Test#3: getUserById
            - GET /users/101
            -   Result
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
            ]
            }
            ```

        -            
-----------------------------------------------------------------------------

### Step 55. Step-05: Implement createOrder RESTful Service.md
-----------------------------------------------------------------------------
-   Step-05: Implement "createOrder" method in OrderController
    - Repository Layer
        - Create OrderRepository
    - Controller Layer: OrderController
        - Method: createOrder
        - POST /users/{userid}/orders         
        
    - Test using Postman
        - Test#1: createOrder 
            - POST /users/101/orders  
            -   Json
            ```json
            {
            "orderDescription": "laptop"
            }
           
            ```
            -   Result
            ```json
            {
                "orderId": 3,
                "orderDescription": "laptop"
            }
            ```
        - Test#2: getAllOrders
            - GET /users/101/orders            
            -   Result
            ```json
             [
                {
                    "orderId": 3,
                    "orderDescription": "laptop"
                },
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

            ```
        - Test#3: getAllUsers
            - GET /users
            -   Result
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
                "orders": [
                    {
                        "orderId": 2,
                        "orderDescription": "asdfas"
                    }
                ]
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
                ]
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
                ]
            }
            ]
            ```
        - Test#4: getUserById 
            - GET /users/101   
            -   Result
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
                    "orderId": 3,
                    "orderDescription": "laptop"
                },
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
-----------------------------------------------------------------------------


### Step 56. Step-06: Implement getOrderByOrderId RESTful Service.md
-   Step-06: Implement "getOrderByOrderId" method in OrderController
    - Controller Layer: OrderController
        - Method: getOrderByOrderId
        - GET /users/{userid}/orders/{orderid}
        
    - Test using Postman
        - Test#1: getOrderByOrderId
            - GET /users/{userid}/orders/{orderid}
            -   Result
            ```json
            {
                "orderId": 2001,
                "orderDescription": "order11"
            }
            ```
-----------------------------------------------------------
-----------------------------------------------------------------------------
### Step 57. Step-07: GIT Commit, Push, Merge to Master and Push.md
------------------
-   Step-07: GIT commit code, push to remote, merge to master and push to remote 
    git status
    git add .
    git commit -am "First Commit - OneToMany"
    git push
    git checkout master
    git merge 06-SpringBoot-JPA-OneToMany
    git branch -vva