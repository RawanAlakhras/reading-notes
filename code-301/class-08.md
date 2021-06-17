# APIs
* What does REST stand for? <br>
Representational State Transfer (REST) as an architectural approach to designing web services .
* REST APIs are designed around resources .
* What is an identifer of a resource? <br>
A resource has an identifier, which is a URI that uniquely identifies that resource .
* REST APIs use a stateless request model .
* POST requests should be based on nouns .
* GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.
* POST creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.
* PUT either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.
* PATCH performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.
* DELETE removes the resource at the specified URL.
## Filter and paginate data
* the API can allow passing a filter in the query string of the URI Which will increase the efficency .
* Also consider imposing an upper limit on the number of items returned .
* Give all optional parameters in query strings meaningful defaults.
