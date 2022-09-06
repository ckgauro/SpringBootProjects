[77]
### Step 77. Step-01: ModelMapper Introduction.md

---------------------------------------------------------------------------
-   Step-00: Introduction
-   Step-02: Update pom.xml with ModelMapper dependency
-   Step-03: Define ModelMapper Bean
-   Step-04: Create a DTO class with name as UserMmDto     
-   Step-05: Create getUserDtoById method with Entity to DTO Conversion logic
-   Step-06: Commit Code (using IDE)
### Step 78. Step-02: ModelMapper Configuration Setup.md
---------------------------------------------------------------------------
-   Step-01: New GIT branch (usign IDE)
    - git Branch name: 10-01-SpringBoot-DTOS-ModelMapper
    - Create new local branch
---------------------------------------------------------------------------
-   Step-02: Update pom.xml with ModelMapper dependency
    - Update pom.xml
        <dependency>
            <groupId>org.modelmapper</groupId>
            <artifactId>modelmapper</artifactId>
            <version>2.3.5</version>
        </dependency>      
---------------------------------------------------------------------------        
-   Step-03: Define ModelMapper Bean
    - Config Layer
        - Create a config package
        - Create AppConfig class
        - Define ModelMapper bean in configuration class
### Step 79. Step-03: Implement Methods using ModelMapper.md

---------------------------------------------------------------------------        
-   Step-04: Create a DTO class with name as UserMmDto    
    - DTO Layer
        - Create UserMmDto with fields userid, username
---------------------------------------------------------------------------        
-   Step-05: Create getUserDtoById method with Entity to DTO Conversion logic
    - Controller Layer
        - Create new controller named UserModelMapperController
        - Annotate with @RestController
        - Annoteate with @RequestMapping("/modelmapper/users")
        - Create getUserDtoById method 
            - GET /{id}    
        - Implement ModelMapper converion logic            
    - Test using Postman   
    -   GET http://localhost:8080/modelmapper/users/102
    ```json
    {
        "id": 102,
        "username": "gwiser",
        "firstname": "Greg",
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
        ]
    }

    ```       
---------------------------------------------------------------------------
-   Step-06: Commit Code (using IDE)
    - Commit code
    - Push branch to Remote repo
### Step 80. Step-04: MapStruct Introduction.md
[80]

### Step 81. Step-05: MapStruct Configuration Setup.md
---------------------------------------------------------------------------
- Step-01: New GIT branch (usign IDE)
    - git Branch name: 10-02-SpringBoot-DTOS-MapStruct
    - Create new local branch
---------------------------------------------------------------------------
- Step-02: Update pom.xml with necessary dependencies for MapStruct
    - pom.xml
**********************************
    - Change#1: Add Properties 
    <properties>
        <org.mapstruct.version>1.3.0.Final</org.mapstruct.version>
        <org.apache.maven.plugins.version>3.8.1</org.apache.maven.plugins.version>
    </properties>
**********************************
    - Change#2: Add mapstruct Depenedency
        <dependency>
            <groupId>org.mapstruct</groupId>
            <artifactId>mapstruct-jdk8</artifactId>
            <version>${org.mapstruct.version}</version>
        </dependency>
**********************************
    - Change#3: Add MapStruct Processor Plugin

            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-compiler-plugin</artifactId>
                <version>${org.apache.maven.plugins.version}</version>
                <configuration>
                    <source>${java.version}</source>
                    <target>${java.version}</target>
                    <annotationProcessorPaths>
                        <path>
                            <groupId>org.mapstruct</groupId>
                            <artifactId>mapstruct-processor</artifactId>
                            <version>${org.mapstruct.version}</version>
                        </path>
                    </annotationProcessorPaths>¬
                 </configuration>
            </plugin>
**********************************     

### Step 82. Step-06: MapStruct - Create UserMapper and Implement getAllUsers Method.md


### Step 83. Step-07: MapStruct - Implement getUserById Method using MapStruct UserMapper.md

