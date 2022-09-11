## Spring Boot -Swagger Integration

-   Documenting REST API is very **important** primarily from API consumers point of view
-   API Documentation helps consumers to understand and implement their client applications without any **confusion** and also by avoiding **costly mistakes**.
-   One of the most popular API documentation specification is **OpenAPI**, formerly known as **swagger**.
-   Swagger allows us to describe API properties either using **JSON** or **YAML** metadata
-   Swagger also provides a **Web UI** which transform the **JSON** metadata to a nice **HTML** documentation
-   SwaggerUI can also be used as a **REST client**.
-   Swagger integration with Spring Framework can be implemented using **SpringFox** dependencies,
 
### Step 92. Step-00: Introduction to Swagger.md
---------------------------------------------------------------------------------------------
Step-00: Introduction
---------------------------------------------------------------------------------------------


### Step 93. Step-01: Add Springfox Dependencies to pom.xml and Create SwaggerConfig file.md
-   Step-01: New GIT branch (usign IDE)
    - git Branch name: 12-SpringBoot-Swagger-APIDocumentation
    - Create new local branch

### Step 94. Step-02: Adding API Info to modify header part of our documentation.md
---------------------------------------------------------------------------------------------
-   Step-02: Add Springfox Dependencies to pom.xml and Restart Embedded Tomcat
		<dependency>
			<groupId>io.springfox</groupId>
			<artifactId>springfox-swagger2</artifactId>
			<version>3.0.0</version>
		</dependency>
		<dependency>
			<groupId>io.springfox</groupId>
			<artifactId>springfox-boot-starter</artifactId>
			<version>3.0.0</version>
		</dependency>
		<!-- https://mvnrepository.com/artifact/io.springfox/springfox-swagger-ui -->
		<dependency>
			<groupId>io.springfox</groupId>
			<artifactId>springfox-swagger-ui</artifactId>
			<version>3.0.0</version>
		</dependency>
		<!-- https://mvnrepository.com/artifact/io.springfox/springfox-bean-validators -->
		<dependency>
			<groupId>io.springfox</groupId>
			<artifactId>springfox-bean-validators</artifactId>
			<version>3.0.0</version>
		</dependency>	

- Step-03: Create SwaggerConfig file
    - Annotate it with @Configuration
    - Annotate it with @EnableSwagger2
    - Create a Docket bean and annotate with @Bean
    - Swagger Metadata URL
        - http://localhost:8080/v2/api-docs
    - Swagger UI URL
        - http://localhost:8080/swagger-ui.html
### Step 95. Step-04: Restrict scope of swagger document generation using API Base packages.md
---------------------------------------------------------------------------------------------
- Step-04: Adding API Info to modify header part of our documentation.
    - Create a new class "ApiInfo"
    - Update the Docket bean with this ApiInfo. 

### Step 96. Step-05: Auto populate documentation for JSR-303 Validations.md


### Step 97. Step-06: Adding Swagger Core Annotations to Model class.md

- Step-05: Restrict scope of swagger document generation using API Basepackages & Paths 
    - Update base package in RequestHandlerSelectors.basePackage
    - Update PathSelectors.ant("/users/**") to limit to specific paths. 
    - Verify in readable format in SWAGGER online editor https://editor.swagger.io/
    - Fix Optional<User> responses. 
    - Test using REST Client of SWAGGER
### Step 98. Step-07: Adding Swagger Core Annotations to Controller classes.md
---------------------------------------------------------------------------------------------
- Step-07: Adding Swagger Core Annotations to Model class
    -  Core Annotations documentation 
        - https://github.com/swagger-api/swagger-core/wiki/Annotations
    - Core Annotations for Model class
        - Class Level: 
            - @ApiModel(description = "Model to create a new user")
        - Field Level: notes, required, position, unordered without position
            - @ApiModelProperty(notes = "userid - Unique identifier of user", required = true, position = 1)
            - @ApiModelProperty(notes = "username of user", required = false, position = 2)
            - @ApiModelProperty(notes = "First name of the User.", example = "Kalyan", required = false, position = 3)
            - @ApiModelProperty(notes = "SSN of the User.", example = "SSN1010", required = true, position = 4)
    - Test
    http://localhost:8080/swagger-ui/index.html


    ---------------------------------------------------------------------------------------------
- Step-08: Adding Swagger Core Annotations to Controller classes
    - Controller Level
        - @Api(tags = "User Management RESTful Services", value = "UserController", description = "Controller for User Management Service")
    - Method Level
        - @ApiOperation(value = "Create a new user")
    - Parameter Level 
        - @ApiParam("User information for a new user to be created.")
    - produces         
---------------------------------------------------------------------------------------------
- Step-09: Commit & Push code via IDE
---------------------------------------------------------------------------------------------

