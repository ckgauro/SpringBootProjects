### Step 1. Step-01: Course Introduction.md

https://github.com/stacksimplify/springboot-buildingblocks

-   ##### Course Content of Spring Boot 2 RESTFul API**
    1.  **Introduction to Spring Boot 2 RESTful APIs**
        -   introduction to Spring Boot along with time evolution

    2.  **Github & HelloWorld**
        https://github.com/stacksimplify/springboot-buildingblocks

    3.  **RESTful APIs with Spring Data JPA & H2**
        -   Database connection
    4.  **Exception Handling with ResponseStatusException**    
        -   Response exception
        
    5.  **Validation & Global Exception Handler**   
        -   Global Exception handler using Controller advise and Rest advise
    6.  **JPA OneToMany Association**
        - Relationship between different tables
    7.  **SpringBoot - HATEOAS**
        -  Relationship link and self link
    8.  **Sprint Boot Internationalization**
        - Internationalize Content according to different language
    9.  **Spring Boot Filtering**
        - Static filtering
        - Dynamic filtering
        - filtering with JSON object

    10. **Spring Boot - DTOS DataTransfer Objects**
        - Data transfer to Object
        - we use map strut and model mapper.

    11. **Spring Boot - Versioning & Content Negotiation**
        -   Version for using   Media, Header, Url
        -   use Content Negotiation

    12. **Spring Boot - Swagger Integration**
        -   Swagger for documentation

    13. **Spring Boot - Actuator & Admin**
        -   Monitoring RESTApis
        -   SpringBoot Admin server

    14. **Spring Boot - Actuator & Micrometer**
        -   Using Micrometer
        -   app Optics
        -   Data series

 
### Step 2. Step-02: Introduction to RESTful API.md
-   Restful WebServices
    -   REST stands for **Representational State Transfer**
    -   Restful Web services  is a **stateless client-server** architecture where web services are **resources** and can be identified by their URIs.
    -   REST **Client applications** can use **GET/POST/PUT/DELETE..** methods to invoke Restful web services,
    -   **LightWeight** and doesn't follow any standards unlike SOAP web services.
-   SOAP vs REST

|SOAP|REST|
|----|----|
|SOAP is a **protocol**| REST is an architectural style|
|SOAP server and Client applications are **tightly coupled and blind with the WSDL contract**| There is **no contract** in REST web services and **client application consuming REST API.|
|Learning curve is **little complex** for SOAP web services| Learning curve is **easy** for REST when compared to SOAP.|
|Rigid **type checking**, binds to a contract.| Human **readable** results|
|SOAP works with **XML** only|REST web services request and response types can be **XML,JSON, text** etc..|

  
### Step 3. Step-03: Development Environment Setup.md

-   Download STS from **spring.io/tools**
-   Open STS and click on Window>Perspective>Open perspective>Other
-   Now open **Git perspective**. Now It will open Git perspective.
 
-   Click on **Clone perspective** and dialog box appear. paste following values
    - URI: "https://github.com/stacksimplify/springboot-buildingblocks"
    - Host : github.com
    -   Repository path: [give you computer location where you want to store]
    -   User: [git user]
    -   Password: [Git password]
-   Click on **Next**. 
    -   Specify Directory path:
        e.g. /Users/ckgauro/Tutorial/github/SpringBootProjects/Master RESTFUL APIs with Spring Boot 2 in 100 Steps/CloneRepository
-   then click on **Finish**
