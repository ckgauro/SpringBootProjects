 ### Spring Boot Actuator
 -  Monitor and Manage Spring Boot Applications using REST/JMX Actuator endpoints
 -  The endpoints offer
    -   Health Check
    -   Meterics Monitoring
    -   Access to Logs
    -   Thread Dumps
    -   Heap Dumps
    -   Envirnomental Info

-   Spring Boot Actuator Endpoints
    -   auditevents
    -   beans
    -   caches
    -   conditions
    -   configprops
    -   env
    -   flyway
    -   health
    -   httptrace
    -   info
    -   integrationgraph
    -   loggers
    -   liquibase
    -   metrics
    -   mappings
    -   scheduletasks
    -   threaddump
    -   Spring MVC, Spring WebFlux or Jersey
    -   heapdump
    -   jolokia
    -   logfile
    -   prometheus
### Step 100. Step-01: Add Actuator Dependency in pom.xml.md
---------------------------------------------------------------------------------------------
Step-00: Introduction
---------------------------------------------------------------------------------------------
Step-01: New GIT branch (usign IDE)
    - git Branch name: 13-SpringBoot-Actuator
    - Create new local branch


### Step 101. Step-02: Expose all Actuator Endpoints and discuss about them.md

---------------------------------------------------------------------------------------------
Step-02: Add SpringBoot Actuator Depenedency in pom.xml
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-actuator</artifactId>
		</dependency>	 
        - Verify the endpoint
            - http://localhost:8080/actuator
        - Only 2 endpoints            
            - health
            - info
        - Other Endpoints (full details)
            - https://docs.spring.io/spring-boot/docs/current/reference/html/production-ready-endpoints.html#production-ready-endpoints

### Step 102. Step-03: SpringBoot Admin Introduction.md

 Step-03: Expose all Actuators endpoints. 
    - application.properties
        - management.endpoints.web.exposure.include=*
    - Verify the endpoints
        - http://localhost:8080/actuator   
    - Health Endpoint
        - management.endpoint.health.show-details=always                

### Step 103. Step-04: SpringBoot Admin - Base Setup.md
Step-04: Info Endpoint
    - Retrieve Build Properties
        - Update pom.xml
			<plugin>
				<groupId>org.springframework.boot</groupId>
				<artifactId>spring-boot-maven-plugin</artifactId>
				<executions>
        			<execution>
            			<id>build-info</id>
            			<goals>
                			<goal>build-info</goal>
            			</goals>
        			</execution>
    			</executions>
			</plugin>
    - Actuator automatically Environment Properties which starts with info in applicaton.properties
        - info.greettings=Good Morning 
    - Info endpoint can gather properties from many spring boot externalized sources.
        - https://docs.spring.io/spring-boot/docs/current/reference/html/boot-features-external-config.html         


### Step 104. Step-05: Point SpringBoot Client Application to SpringBoot Admin Server.md

Step-05: Metrics Endpoint
    - Metrics
        - http://localhost:8080/actuator/metrics
        - http://localhost:8080/actuator/metrics/jvm.memory.used
        - http://localhost:8080/actuator/metrics/jvm.threads.states
        - http://localhost:8080/actuator/metrics/http.server.requests  
--------------------------------------------------------------------------------------------
    

### Step 105. Step-06: Test the features in SpringBoot Admin Server.md
### Step 106. Step-00: SpringBoot Actuator Introduction.md
