![Alt text](https://www.accenture.com/content/dam/accenture/final/images/icons/symbol/Acc_Logo_Black_Purple_RGB.png?raw=true "Accenture")
# Accenture Hiring Challenge
***
## Table of Contents
1. [Introduction](#introduction)
2. [Project Structure and Current Functionality](#project-structure-and-current-functionality)
3. [What You Will Do](#what-you-will-do)
4. [How To Test Your Endpoints](#how-to-test-your-endpoints)
***
### Introduction
Welcome to the **Accenture Hiring Challenge**!, This file contains all the information you need to know about the project.
This Project consist of an API made with Spring Boot and JPA.  For this project, you will need to implement the missing 
functionality in the project. To get the code, ***fork*** this repository, and ***clone*** it into a local repository. Once you have done this, you are ready to start
coding!
***
### Project Structure and Current Functionality
The flow of the project is the following:

![Project Flow](C:\Users\luis.meza\Pictures\projectFlow.jpeg)

In the image above, we can see that:
- A call is made to the API, which will be available when the server is running. By default, the API will run on **port 8080**. The call of the API is handled by the ***Controller*** class, which will get information about the call, like, http method, path parameters, variables, request body, etc.
- The ***Controller*** class calls the ***Service*** class, where the business logic is implemented.
- Then, the ***Service*** class calls the ***Repository*** interface, the repository will simplify the query of data in the database.
- Finally, the data is stored in the **Database**, and the application returns a response depending on the result of the operation.

The current project folder structure is the following:

![Project Structure](C:\Users\luis.meza\Pictures\projectStructure.png)

Where the ***Controller***, ***Service***, and ***Dao*** folders contain the **Controller** class, **Service** class and interface, and **Repository** interfaces respectively.
The ***Dto*** and ***Model*** folder contain the **Dto (Data Transfer Object)** and the **Model** classes for the ***Course*** entity. The actual class that is persisted in the API is the **Model** class, the Dto is used to optimize responses and transfer of objects.

Currently, the project just has the ***Course*** entity with its GET and DELETE
methods.

In image above, right at the bottom, we can see the Unit Testing package, here, you will create your Unit Tests for each implementation that you create.

***
### What You Will Do
Your job is to implement the ***create***, ***update*** and ***get one*** methods functionality (POST, PUT and GET) for the **Course** entity,
as well as its respective Unit Tests.

***
### How To Test Your Endpoints
To test your implementations and endpoints, you need to follow the next steps (This applies for all endpoints):
- Open Postman
- Go to the "login" endpoint
- Create a request with the GET method and send the following credentials in the request body:
  - user: admin
  - password: admin
- The application will return a Bearer Token, save it or copy it wherever you want
- Use the Bearer Token returned by the application in every endpoint you want to test
***
#### Good luck!