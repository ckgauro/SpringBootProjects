### Step 4. Step-00: Best way to quickly complete this course.md


### Step 5. Step-00: Github & HelloWorld Introduction.md
-   Step-00: Github & HelloWorld Introduction
-   Step-01: Create Spring boot base project from start.spring.io
-   Step-02: Introduction for managing spring boot projects via github
-   Step-03: Github Base Setup
-   Step-04: Add GIT Repository to Spring Tool Suite IDE -  GIT Perspective
-   Step-05: Create a Simple HelloWorld RESTful API which returns a String
-   Step-06: Create a Simple Hello World REST Service which returns a Bean (JSON)
-   Step-07: GIT Commit & Push Hello World RESTful service changes to Github
### Step 6. Step-01: Create Spring Boot base project from start.spring.io.md
-   Create a SpringBoot Project with required Dependices
    1.  Create Project in **https://start.spring.io** and import to Intellij.
        -   Spring Boot starter Web
        -   Spring Boot Dev tools
        -   Spring Data JPA
        -   H2 Database
    2.  Verify Dependencies in pom.xml
        -   spring-boot-starter-data-jpa
        -   spring-boot-starter-web
        -   spring-boot-starter-devtools
        -   h2
        -   lombok

    3.  Run the app / start the App as Spring Boot App and verify if it comes up.

### Step 7. Step-02: Introduction for managing Spring Boot projects via github.md
https://github.com/ckgauro/springboot-buildingblocks

Step-03: Manage SpringBoot project via github GIT Repository 
For every major step, we follow below steps from GIT perspective
    1.  Checkout code to new branch from master
    2.  Make changes or add code
    3.  Commit code to local branch
    4.  Push code to remote branch
    5.  checkout to master
    6.  Merge to master
    7.  Push code to remote master

Base Setup - Steps      
    1.  Create a project on github

Master Branch
    2.  Initiate Local Repository
    3.  Create master branch
    4.  check-in code
    5.  Add GIT Remote origin
    6.  Push code to remote branch
    7. Verify in remoe branch

01-ground-zero branch
    7.  create 01-ground-zero branch
    8.  Push code to remote branch

Add Repo to IDE GIT Perspective
    9.  Add this git repository on STS IDE GIT Perspective and Verify            
### Step 8. Step-03: Github Base Setup.md 
- Done
```
git init
git add .
git status
git commit -am "first commit"
git status
git remote add origin https://github.com/ckgauro/springboot-buildingblocks.git
git push -u origin master
git push --set-upstream origin master

git status 
$ git checkout -b 01-ground-zero-base
Switched to a new branch '01-ground-zero-base'

git push --set-upstream origin 01-ground-zero-base
```
### Step 9. Step04: Add GIT Repository to Spring Tool Suite IDE.md
- Done

Open GIT repository in Intellij
https://github.com/ckgauro/springboot-buildingblocks.git

-   add Git Staging


### Step 10. Step05: Create a Simple Hello World RESTful Service which returns a String.md

```
    $git branch
    $git show-branch
    $git checkout master
    $git status
    $git branch
    $git merge 01-ground-zero-base
    $git push
    [Now check in https://github.com/ckgauro/springboot-buildingblocks.git we can find master and  01-ground-zero-base has same hash value]


 $ git checkout -b 02-Hello-world
M       springboot-buildingblocks/pom.xml
Switched to a new branch '02-Hello-world'
$ git status
On branch 02-Hello-world
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   springboot-buildingblocks/pom.xml

no changes added to commit (use "git add" and/or "git commit -a")

    $git push --set-upstream origin 02-Hello_world

[STS File>Refresh it will display]
[Now check in https://github.com/ckgauro/springboot-buildingblocks.git we can find 02-Hello_world]

```

Step-04: Hello World Rest Service
4-A:
    -   Create git branch "02-Hello-World"
    -   Create a HelloWorld Controller
        -   Create a simple Method which returns string "Hellow World"
        -   Controller: @RetController
        -   Mapping - @RequestMapping GET & Path "/hellowworld"
        -   Mapping - @GetMapping &Path "/helloworld"

4-B:
    -   Create a method which returns Bean
        -   Create a simple Method which returns a bean with some content (firstname, lastname, city) in JSON
        -   Mapping - @RequestMapping GET & Path "/hellowworld-bean"
        -   Mapping - @GetMapping &Path "/helloworld-bean"
  
4-C: 
    -   GIT PUSH (Command Line)
        -   Commit and Push code to remote repo
        -   Merge with Master and push code to remote repo
### Step 11. Step-06: Create a Simple Hello World REST Service which returns a Bean (JSON).md

- Branch [02-Hello-World]
https://github.com/stacksimplify/springboot-buildingblocks/blob/02-Hello-World/src/main/java/com/stacksimplify/restservices/Hello/HelloWorldController.java
#### Test
```
http://localhost:8080/helloworld
Hello World
```

https://github.com/stacksimplify/springboot-buildingblocks/blob/02-Hello-World/src/main/java/com/stacksimplify/restservices/Hello/UserDetails.java

#### Test
```
http://localhost:8080/helloworld-bean

{
  "firstName": "Mina",
  "lastName": "Reddy",
  "city": "KTM"
}

```

 
### Step 12. Step-07: GIT Commit & Push Hello World RESTful service changes to Github.md

$git status
$git add .
$git status
$git commit -am "Hello World Base"
$git show-branch
$git push
$git checkout master
$git merge 02-Hello-World
$git push
   [Now check in https://github.com/ckgauro/springboot-buildingblocks.git we can find master and  02-Hello-World has same hash value]

```
$ git status
On branch 02-Hello-world
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   springboot-buildingblocks/pom.xml

no changes added to commit (use "git add" and/or "git commit -a")
$ git status
On branch 02-Hello-world
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/HelloWorldController.java
        new file:   springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/UserDetails.java

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   springboot-buildingblocks/pom.xml
        modified:   springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/HelloWorldController.java
        modified:   springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/UserDetails.java

$ git add .
$ git status
On branch 02-Hello-world
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   springboot-buildingblocks/pom.xml
        new file:   springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/HelloWorldController.java
        new file:   springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/UserDetails.java

$ git commit -am "Hello World Base"
[02-Hello-world 73f6416] Hello World Base
 3 files changed, 45 insertions(+), 1 deletion(-)
 create mode 100644 springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/HelloWorldController.java
 create mode 100644 springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/UserDetails.java
$ git show-branch
! [master] master
 ! [01-ground-zero-base] master
  * [02-Hello-world] Hello World Base
---
  * [02-Hello-world] Hello World Base
++* [master] master
$ git push
fatal: The current branch 02-Hello-world has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin 02-Hello-world

$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.
$ git merge 02-Hello-World
Updating be871a9..73f6416
Fast-forward
 springboot-buildingblocks/pom.xml                                                                                                    |  1 -
 springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/HelloWorldController.java | 26 ++++++++++++++++++++++++++
 springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/UserDetails.java          | 19 +++++++++++++++++++
 3 files changed, 45 insertions(+), 1 deletion(-)
 create mode 100644 springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/HelloWorldController.java
 create mode 100644 springboot-buildingblocks/src/main/java/com/gauro/restservices/springbootbuildingblocks/restservices/hello/UserDetails.java
$ git push
Enumerating objects: 25, done.
Counting objects: 100% (25/25), done.
Delta compression using up to 12 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (15/15), 1.44 KiB | 1.44 MiB/s, done.
Total 15 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/ckgauro/springboot-buildingblocks.git
   be871a9..73f6416  master -> master
$ 

```