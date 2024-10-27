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
