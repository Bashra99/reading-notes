# API

**What does REST stand for?**
Representational State Transfer (REST) as an architectural approach to designing web services. REST is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP.
 
 **REST APIs are designed around a resources.**
**What is an identifier of a resource? Give an example.**
https://www.sciencedirect.com/topics/computer-science/resource-identifier
**What are the most common HTTP verbs?**

GET, POST, PUT, PATCH, and DELETE.
**What should the URIs be based on?**

resources.

**Give an example of a good URI.**
**What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**

An API which makes alot of requests and it is bad.

**What status code does a successful GET request return?**

status code 200 (OK)

**What status code does an unsuccessful GET request return?**

If the resource cannot be found, the method should return 404 (Not Found).

**What status code does a successful POST request return?**

status code 201 (Created).
**What status code does a successful DELETE request return?**
204 
## References
<https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design>
