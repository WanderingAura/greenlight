# Greenlight
A CRUD JSON API server for listing movies. The code is from the guided project in the book Let's GO Further by Alex Edwards.

The API implements basic authentication and permissions for users. When a user registers using the `/v1/users` POST endpoint, an activation is email is sent to them. Registered users are able to view movies but not add movies. Activated users can add movies to the database.

A rate limiter based on IP address has been implemented as part of the middleware chain to prevent spam.