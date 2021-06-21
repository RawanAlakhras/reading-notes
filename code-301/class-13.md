# CRUD

* 100-199 - This refers to the header being received from the client by the server and the server will begin to work through the request. The server will tell the client whether it passed or failed.

* 200-299 - Success, request received.

* 300-399 - Redirection. Resource unavailable or not at expected location. 400-499 - Error. Invalid request from client to server. (timeouts, missing information, etc)

* 500-599 - Server Error - Commonly referring to overloaded and/or servers not reachable. Sometimes from a client request.

* 308 - Permanent Redirect - States that there has been a permanent redirect, change to the location. Resource has been moved to the url stated in location header.

* 204 - No Content - Updates returning no content beck to the client that requested the data.

* 410 - Gone - This resource used to exist but is now gone. The implication is that the server knows that it used to exist.

* 403 - Forbidden - Server understood but denied (did not authorize) the request.

## What is a status code 202?

* Accepted, This code tells the client that the request was valid

## What is a status code 308?

* Permanent Redirect ,This tells the client to use another URL to access the resource and not use the current URL anymore.

## What code would you use if an update didn’t return data to a client?

* 204 No Content

## What code would you use if a resource used to exist but no longer does?

* 414 Request-URI Too Long

## What is the ‘Forbidden’ status code?

* 404 Not Found

## What is the difference beween PUT and PATCH?

* patch : when we need to update based on what the user passes us put : it will update all the info to describe it all at once instead of the info that gets passed

* How do you make a defalut value in a schema? <br>
so we are just going to use default and set this to date.now ,if we don’t pass our date it is just going to default it to current date