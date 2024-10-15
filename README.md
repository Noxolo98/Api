Simple REST API
Welcome to the repository for my simple REST API. This API provides basic CRUD (Create, Read, Update, Delete) operations for managing subjects.

Table of Contents
Overview
Technologies
Installation
Usage
Endpoints
Testing

OVERVIEW:
This REST API supports the following operations:

Create: Add a new subject
Read: Retrieve subjects
Update: Modify existing subjects
Delete: Remove a subject

TECHNOLOGIES:
Backend Framework:(Node.js/Express.)]
API Testing: Postman 

INSTALLATION:
1. git clone https://github.com/Noxolo98/Api.git
cd Api
2. npm install
3. npm start

The API will start on http://localhost:3000 or another port if configured.

USAGE:

# get all subjects
 http://localhost:3000/subjects

# Get a subject by ID
 http://localhost:3000/subjects/1

# Create a new subject
POST "Content-Type: application/json" -d '{"name": "New subject", "description": "Details here"}' http://localhost:3000/subjects

# Update a subject by ID
PUT "Content-Type: application/json" -d '{"name": "Updated subject", "description": "Updated details"}' http://localhost:3000/subjects/1

# Delete a subject by ID
DELETE http://localhost:3000/subjects/1

ENDPOINTS:

Endpoints
GET /subjectss
Description: Fetch all subjects.
Response: A list of subjects.
GET /subjects/:id
Description: Fetch a subject by ID.
Response: A single subject object.
POST /subjects
Description: Create a new subject.

Body (JSON):
{
  "name": "subject name",
  "description": "subject description"
}

PUT /subjects/:id
Description: Update an existing subject.
Body (JSON):
{
  "name": "Updated name",
  "description": "Updated description"
}
DELETE /subjects/:id
Description: Delete a subject by ID.

TESTING:

To test the API use Postman. 









