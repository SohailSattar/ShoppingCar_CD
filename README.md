# Shop API
Assesement task.

## Description
A store requires a an API to add, remove, update or read the cart item(s). This API uses in-memory database to store records. By default, some random values has been added in the shopping cart to play with.

For security, JWT Authentication is used.

## Technologies / Tools used
This project is built in Dotnet Core 3.1 using C# programming language and SQL Server for data stoage. Apart from it, following tools/technologies have been added too:
* **Entity Framework Core** for easy data reading and manipulation and for clean code.
* **Swagger UI** for visual rendering of API documents
* **Dependency Injection** is also being used to totally seperate the functionalities of individual classes.
* **JWT** for authorizations.


### WebAPI
1: Download the API project.
2. Open it in Visual Studio.
3. Build the application and run it.
4. By default, /api/cart-items GET request will be hit with 401 unauthorized access i.e. the user is not logged in yet. To be able to see the records, call the /api/token POST request and enter following details in JSON format:
          {
              "email":"admin@bookshop.com",
              "password":"admin"
          }
  Please note that these are hard coded values because our storage choice was in-memory database.
5. If the request is valid, a valid 200 response will be returned with the email and the valid token, use that token to access the GET, POST, PUT and DELETE requests.
