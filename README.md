# API Documentation

This document provides a detailed overview of the API for the shopping application. It includes information about authentication, product management, shopping cart operations, and order processing.

## Table of Contents

- [Base URL](#base-url)
- [Authentication Endpoints](#authentication-endpoints)
- [Product Management Endpoints](#product-management-endpoints)
- [Shopping Cart Endpoints](#shopping-cart-endpoints)
- [Order Management Endpoints](#order-management-endpoints)
- [Error Handling](#error-handling)
- [Authentication and Authorization](#authentication-and-authorization)
- [Input Validation](#input-validation)

## Base URL

The base URL for the API is:
http://localhost:5000/api



## Authentication Endpoints

### 1. Register a New User

- **Endpoint**: `POST /auth/register`
- **Request Body**:
  ```json
  {
    "userName": "string",
    "email": "string",
    "password": "string"
  }

- **Description**: Registers a new user.

### 2. Log In User
-**Endpoint**: `POST /auth/login`
- **Request Body**:
  ```json
  
  {
  "email": "string",
  "password": "string"
  }


- **Description**: Logs in a user and returns authentication tokens.

### 3\. Log Out User

*   **Endpoint**: POST /auth/logout
    
*   **Request Body**: None
    
*   **Description**: Logs out the current user.
    

### 4\. Check Authentication Status

*   **Endpoint**: GET /auth/check-auth
    
*   **Request Body**: None
    
*   **Description**: Checks if the user is authenticated.
    

Product Management Endpoints
----------------------------

### 1\. Get Filtered Products

*   **Endpoint**: GET /shop/products/get
    
*   **Request Body**: None
    
*   **Description**: Retrieves a list of filtered products.
    

### 2\. Get Product Details

*   **Endpoint**: GET /shop/products/get/:id
    
*   **Request Body**: None
    
*   **Description**: Retrieves details of a specific product by ID.
    

Shopping Cart Endpoints
-----------------------

### 1\. Add Item to Cart

*   **Endpoint**: POST /shop/cart/add
    
*   **Request Body**:
