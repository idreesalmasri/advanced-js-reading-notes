## Dynamic API Server
An Express/Node.js based server designed to be a “model agnostic” REST API server, which can perform CRUD operations on any data model

Support all REST/HTTP methods
- GET: Retrieve record(s) from a data source
>All  
One (by id)  
Some (by filtering)  
- POST: Create a new record in a data source
- PUT: Update a single full record in a data source
- PATCH: Update part of a single record in a data source
- DELETE: Delete a record in a data source  

### Obey a standard output format
- Results will be returned in JSON format
- Results will be served with the correct HTTP header - application/json
- The GET Route, when not retrieving by ID, must return a full header, with count ,pages, and a results array
- All other routes must return a single object, representing the state of the entity following the operation


### Development Process, Milestones
#### Phase 1: Basic Authentication

 _ Use JSON Server (non-express) to mock the routes for testing purposes

#### Phase 2: Bearer Authentication

- Create CRUD/ReST endpoints for categories and products
- Separate route modules for each data model type
- Store user created data in memory (no persistence)
- Integrates with an online CI framework
#### Phase 3: Authorization
- Replace the in-memory data store with mongo
- Use Mongo Collections for each data model type

## Authentication Server / Module
### Development Process, Milestones
1- Phase 1: Basic Authentication
Create a basic express server with the following features:
- Users Model (Mongoose Schema)
- /signup route that creates a user
- /signin route that attempts to log a user in
- BasicAuth middleware that validates the user as a part of the /signin process
Implement: Modularize and Test a starter server

2 -Phase 2: Bearer Authentication
- Re-Authenticate Users
- Accepts a TOKEN in the Authorization: Bearer header
- Validates the user
- Allows or Denies access to the route handler
- Implement: Debug, Extend Token Security

3 Phase 3: Authorization
- Role Based Authorization System
- Combines the Bearer Token with User roles to give fine grained access control
- Implement: Protect API Routes, Write tests