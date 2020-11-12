# Description

- This repository is intended to have a `common/shared` library of workflows
- There are several `yaml` files in the root of this repository
  - Each `yaml` file is intended to be a workflow which does something that can be applied to multiple repositories (for example building/testing a java project)
- The repository has its own workflow which synchronizes these `yaml` files into other repositories
  - These repositories are specified in the workflow definition
 
 > The takeaway is that we can share certain workflows instead of repeating the same thing over and over again
 
 For the purpose of this demo the following 3 repositories are used:
 - https://github.com/AlexandruGodri/java-demo-1
 - https://github.com/AlexandruGodri/java-demo-2
 - https://github.com/AlexandruGodri/java-demo-3
 
 The java projects are dummy Spring Boot projects with java 8, 11 and 15.
 
 Whenever something is pushed in this repository the workflows are being updated in those 3 java projects.
 
