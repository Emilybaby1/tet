# Online-Bookstore-API-Team-12

## Table of Contents
* Introduction
* Terminologies Used
* Prerequisites
* Getting Started
* Contibutors
* User Guide


## Introduction

Welcome to the online book store project. This API provides a comprehensive and user-friendly guide that would aid in navigating your way on the online book store system. It enables users to register, login,view,search for available books and purchase them.Even if you are a user eager to explore the functionalities or a developer intergrating with the API.

Admins Have Following Access for this online store site:
* Add New Books.
* View Books Available.
* Remove Books.

Users Have Following Access for this online store site:
* Register or Create a New Account.
* Login.
* View Books Available.
* Search for Books. 
* Add a book to cart.
* Remove a book from cart.
* Purchase Books.

## Terminologies Used

The Online Book Store API used the following terminologies 

* C# and .NET technologies
* ASP.NET Core
* Entity Framework Core
* JWT (JSON Web Tokens) for authentication
* Microsoft Identity for user management
* Microsoft SQL Server for the database

## Prerequisite

In other to run this project you'll need 
* Browser
* VS Code or any code editor


## Getting Started

Ensure to Download the Necessary Requirement and Dependencies installed before beginning the setup 

or

get a local copy running by clicking on this site

`https://github.com/Codevixens-Band-3-General-Project/Online-Bookstore-API-Team-12.`



## Contributors
* Abiola Abdulsalam		
* Chepngeno Jackline

## User Guide

1. Create a Repository 

2. Clone the Repository:
You can clone the repository using this 

`git clone <repository_url> `


   Replace the `<repository_url>` with the Url of the github repository you want to clone.

   eg 

  ` git clone https://github.com/yourusername/repository.git`
  
3. Then Install dependencies to
    
`   cd online-book-store-api

   dotnet restore
`
  This code would only restore the package but won't build it.

4. Configure the database

* Open the `appsettings.json` file. 

* Modify the `ConnectionStrings:DefaultConnection` value to match your SQL Server connection string.

* Modify the `JwtConfig:Secret` value to use a secure key for JWT token generation. it is recommended to generate a strong random key of sufficient length(e.g, 256bits)

5. Apply database migrations
   
   `dotnet ef database update`

6. Run the API
   
   `dotnet run`

7. Explore the API endpoints
   
* The API is now running locally on `**http://localhost:5000.**`

* Use a tool like Postman or cURL to make HTTP requests to the available endpoints. 

* Go to the API Documentation for detailed information about the endpoints and their usage.


8. User Authentication
    
* Register a new user by making a `POST` request to `/authentication/register` with the required `user` details.
  
* Obtain a JWT token by making a `POST` request to` /authentication/login ` with the user's `login` credentials. The token will be included in the response.
  
* Include the obtained JWT token in the` Authorization header` for authenticated requests. Example:` Authorization: Bearer <token>`


9. Manage Books
    
* Use the appropriate endpoints to perform CRUD operations on books, such as creating, updating, deleting, and retrieving books by various criteria.
  
* Ensure you have the necessary authorization roles to access specific endpoints.
  
* Admin privileges are required for certain operations.

10. Shopping Cart
    
* Add books to the shopping cart using the `/book/add-to-cart/{id}` endpoint.

* View the contents of the shopping cart using the ` /book/view-cart` endpoint.
  
* Remove books from the shopping cart using the `/book/delete-from-cart/{id}` endpoint.
  
11. Error Handling
    
The API includes robust error handling mechanisms to provide meaningful error messages and responses in case of exceptions or invalid requests.

12. Logging

Logging is implemented to capture relevant information for debugging and troubleshooting purposes. Check the log files for any issues or helpful insights.

## 
The steps mentioned above should provide you with the resources you need to do research and take part in the project. 
Do not hesitate to contact us if you have any questions or recommendations. It's fun to code!
Happy Coding.

