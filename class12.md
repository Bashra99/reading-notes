## Readings: CRUD

### Status Codes Based On REST Methods

- 100’s = informational status codes; request will fail before they start sending the body.
- 200’s = success codes; request accepted.
- 300’s = redirection codes; not available.
- 400’s = error codes; invalid requests .
- 500’s = server error codes; overwhelmed servers or unreachable servers.

### What is a status code 202?

- asynchronous processing.

### What is a status code 308?

- Permanent Redirect; indicates that other url should be used.

### What code would you use if an update didn’t return data to a client?

- 204

### What code would you use if a resource used to exist but no longer does?

- 410

### What is the ‘Forbidden’ status code?

- 403

## Build A REST API With Node.js, Express, & MongoDB - Quick

### Why do we need to pull our MongoDB database string out of our server and put it into our .env?

- for storing sensitive data (not to be pushed)

### What is middleware?

- system with functions that have access to the request object (req), the response object (res), and the next function in the application’s request-response cycle. The next function is a function in the Express router which, when invoked, executes the middleware succeeding the current middleware.

### What does app.use(express.json()) do?

- allow us to use express methods.

### What does the /:id mean in a route?

- id is the unique instance field (_id) that is given to each Mongoose model instance by default.

### What is the difference beween PUT and PATCH?

- PUT = create , PATCH = update

### How do you make a defalut value in a schema?

- by creating a new document without that path set, the default will kick in.

### What does a 500 error status code mean?

- 500 Internal Server Error

### What is the difference between a status 200 and a status 201?

- 200 = accessible resource, 201 = create operations
