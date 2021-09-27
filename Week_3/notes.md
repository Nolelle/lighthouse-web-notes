### Note

Since HTTP is a request/response protocol, there is only one reponse per request.
We may encounter error that is console log but does not crash the program (HTTP headers...).
This means we have two res.sends in the response, meaning we cant do the second request because there was only one request, therefore only one response.
To stop that make sure we return our res.send(), this stops the response so we dont go into the second send function and console.log the HTTP error.
