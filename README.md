# JWT Authentication in ASP.NET Core

This guide explains how to add, configure, and test JWT authentication in an ASP.NET Core API using Postman.

## Overview
We will create an API controller named `HomeController` with three key actions:

1. **Login**: This action will simulate a login using a fictitious username and password. If the credentials are correct, a JWT token will be generated and returned.
2. **Admin**: This action will only be accessible with a valid JWT token.
3. **GenerateJwtToken**: A private method responsible for generating the JWT token after validating user credentials.

Additionally, we will create a `LoginModel` class to handle login requests.

## Configuration Steps

### 1. Implement `LoginModel` Class
Create a `LoginModel` class to manage login requests.

### 2. Configure `appsettings.json`
Define the JWT settings in the configuration file.

### 3. Implement `HomeController`
Create an API controller with login and protected endpoints.

### 4. Configure JWT in `Startup.cs`
Modify `ConfigureServices` in `Startup.cs` to add JWT authentication.

### 5. Testing with Postman
#### **Step 1: Obtain a Token**
Send a `POST` request to the login endpoint with the necessary credentials to receive a JWT token.

#### **Step 2: Access Protected Route**
Use the obtained token to access the protected admin route by including it in the request headers.

## Conclusion
This setup enables JWT authentication in ASP.NET Core, ensuring secure access to protected routes. You can now extend this implementation for real-world authentication scenarios.

