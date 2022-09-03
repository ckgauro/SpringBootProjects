
### Step 66. Step-00: Introduction to Internationalization.md

-----------------------------------------------------------------------------
Step-00: Introduction
-----------------------------------------------------------------------------
Step-00: New GIT branch for Internationalization
git branch -vva
git status
git checkout -b 08-SpringBoot-Internationalization
git push --set-upstream origin 08-SpringBoot-Internationalization
git branch -vva
### Step 67. Step-00: Create git branch for Internationalization.md

### Step 68. Step-01: Create LocaleResolver and ResourceBundleMessageSource Beans.md

-----------------------------------------------------------------------------
Step-01: Create required beans
    - Define a Bean named LocaleResolver
    - Add messages.properties, messages_fr.properties
    - Define a Bean named ResourceBundleMessageSource  
### Step 69. Step-02: Implement RESTful Service with Internationalization.md

-----------------------------------------------------------------------------
Step-02: Create a REST service which supports i18n
    - Create a helloi18n Method in HelloWorldController
    - Test it via Postman with "Accept-Language" headers
        - Accept-Language: fr 
        - Accept-Language: us
        - Accept-Language: en 

### Step 70. Step-03: GIT Commit, Push, Merge to Master and Push.md

-----------------------------------------------------------------------------
Step-03: GIT commit code 
git status
git add .
git commit -am "First Commit - Internationalization"
git push
git checkout master
git merge 08-SpringBoot-Internationalization
git branch -vva
-----------------------------------------------------------------------------