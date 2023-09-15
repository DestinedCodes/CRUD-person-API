# CRUD Person API Documentation

## Overview

The CRUD Person API is designed to facilitate the management of person records. It provides endpoints for creating, retrieving, updating, and deleting person entries.

### UML and ER Diagrams
#### UML Diagram
![UML (1)](https://github.com/DestinedCodes/CRUD-person-API/assets/84413505/7844d023-fa53-4934-b5a1-ef83cfd74cea)

#### ER Diagram
![ER](https://github.com/DestinedCodes/CRUD-person-API/assets/84413505/8fe4e697-920e-47ff-9bc5-802b42947e81)

## Request Format

### Create a Person (POST)

- URL: `/api`
- Method: POST
- Request Body: `{ "name": "John Doe" }`
- Headers: None
- Response: `<name> created successfully` or `<specific error message>`

### Get a Person by ID (GET)

- URL: `/api/<int:user_id>`
- Method: GET
- Request# CRUD Person API Documentation

### Update a Person by ID (PUT/PATCH)

- URL: `/api/<int:user_id>`
- Method: PUT or PATCH
- Request Body: `{ "name": "Updated Name" }`
- Headers: None
- Response: `<name> updated successfully` or `404 Not Found`

### Delete a Person by ID (DELETE)

- URL: `/api/<int:user_id>`
- Method: DELETE
- Request Body: None
- Headers: None
- Response: `200 OK` or `404 Not Found`

## Response Format

Responses are provided in JSON format and include appropriate HTTP status codes.

## Assumptions and Limitations
- The maximum name length is 50 characters.
- The Person's name contains only valid characters letters, numbers and spaces.

## Setup and Deployment Instructions

For step-by-step instructions on setting up and deploying the API, please consult the README.md file.
