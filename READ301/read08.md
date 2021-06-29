# RESTful web API design
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRgvkrA8vmiQQDeI_PopVicVu2aK5n5MImxAg&usqp=CAU)
###  I want to know more about RESTful web API design
#### designed web API should aim to support:
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRCup90pGg46a83dHVT65Fi5qe5tE5yCdHxeA&usqp=CAU)
- Platform independence:
 Any client should be able to call the API, regardless of how the API is implemented internally. This requires using standard protocols, and having a mechanism whereby the client and the web service can agree on the format of the data to exchange.
- Service evolution:
 The web API should be able to evolve and add functionality independently from client applications. As the API evolves, existing client applications should continue to function without modification. All functionality should be discoverable so that client applications can fully use it.
 **What is REST?**
 In 2000, Roy Fielding proposed Representational State Transfer (REST) as an architectural approach to designing web services. REST is an architectural style for building distributed systems based on hypermedia. 
 EST is independent of any underlying protocol and is not necessarily tied to HTTP.
 ####  some of the main design principles of RESTful APIs using HTTP:
 - REST APIs are designed around resources.
 - A resource has an identifier, which is a URI that uniquely identifies that resource.
 - Clients interact with a service by exchanging representations of resources. 
 - REST APIs use a uniform interface, which helps to decouple the client and service implementations.
 - REST APIs use a stateless request model.
 - REST APIs are driven by hypermedia links that are contained in the representation. 
 ## Organize the API design around resources
 A resource doesn't have to be based on a single physical data item,Avoid creating APIs that simply mirror the internal structure of a database.
 **The purpose of REST** is to model entities and the operations that an application can perform on those entities. A client should not be exposed to the internal implementation.
 Entities are often grouped together into collections (orders, customers). A collection is a separate resource from the item within the collection, and should have its own URI. 
 Sending an HTTP GET request to the collection URI retrieves a list of items in the collection. Each item in the collection also has its own unique URI. An HTTP GET request to the item's URI returns the details of that item.
 #### Define API operations in terms of HTTP methods
 - GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.
 - POST creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.
 - PUT either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.
 - PATCH performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.
 - DELETE removes the resource at the specified URI.
 #### The differences between POST, PUT, and PATCH can be confusing
 A POST request creates a resource. The server assigns a URI for the new resource, and returns that URI to the client. In the REST model, you frequently apply POST requests to collections.
 A PUT request creates a resource or updates an existing resource. The client specifies the URI for the resource. The request body contains a complete representation of the resource. 
 A PATCH request performs a partial update to an existing resource. The client specifies the URI for the resource. The request body specifies a set of changes to apply to the resource. 
 ## Asynchronous operations:
 Sometimes a POST, PUT, PATCH, or DELETE operation might require processing that takes a while to complete. If you wait for completion before sending a response to the client, it may cause unacceptable latency. If so, consider making the operation asynchronous. Return HTTP status code 202 (Accepted) to indicate the request was accepted for processing but is not completed.
 #### Filter and paginate data
 xposing a collection of resources through a single URI can lead to applications fetching large amounts of data when only a subset of the information is required. 
 #### Support partial responses for large binary resources
 A resource may contain large binary fields, such as files or images. To overcome problems caused by unreliable and intermittent connections and to improve response times, consider enabling such resources to be retrieved in chunks. To do this, the web API should support the Accept-Ranges header for GET requests for large resources.
 #### Use HATEOAS to enable navigation to related resources
ne of the primary motivations behind REST is that it should be possible to navigate the entire set of resources without requiring prior knowledge of the URI scheme. Each HTTP GET request should return the information necessary to find the resources related directly to the requested object through hyperlinks included in the response, and it should also be provided with information that describes the operations available on each of these resources. 
#### Versioning a RESTful web API
As business requirements change new collections of resources may be added, the relationships between resources might change, and the structure of the data in resources might be amended. While updating a web API to handle new or differing requirements is a relatively straightforward process, you must consider the effects that such changes will have on client applications consuming the web API.
#### URI versioning
Each time you modify the web API or change the schema of resources, you add a version number to the URI for each resource. The previously existing URIs should continue to operate as before, returning resources that conform to their original schema.
## Header versioning
Rather than appending the version number as a query string parameter, you could implement a custom header that indicates the version of the resource.