<h1 style="text-align=center">
<img src="./images/dothack.jpg" height=50/> .Hack API Workshop</h1>

> Things to do before the workshop:
> Install <a href="https://www.postman.com/download">Postman</a> or <a href="https://insomnia.rest/download/" target="_blank">Insomnia Core</a>
>
> In your command line run this
>  - ```pip install requests```


<br>

# Intro to REST API
### Whats a API?
- Application Programming Interface
  - A set of functions and procedures allowing the creation of applications that access the features or data of an operating system, application, or other service.
- TLDR, API is a thing where your client program can interact with to get stuff(Get Data) or do stuff(Add Data to Database)

### What about the "REST" part?
- Representational State Transfer
  - A set of rules that developers follow when creating their API.

- REST Guidelines
    - REST APIs are stateless, meaning that calls can be made independently of one another, and each call contains all of the data necessary to complete itself successfully. 
    - A REST API should not rely on data being stored on the server or sessions to determine what to do with a call, but rather solely rely on the data that is provided in that call itself. Identifying information is not being stored on the server when making calls. 
    - Instead, each call has the necessary data in itself, such as the API key, access token, user ID, etc. This also helps increase the API’s reliability by having all of the data necessary to make the call, instead of relying on a series of calls with server state to create an object, which may result in partial fails. 
    - Instead, in order to reduce memory requirements and keep your application as scalable as possible, a RESTful API requires that any state is stored on the client—not on the server.

    - **You should be able to get a piece of data when you link to a specific URL.**
  
- Examples
  - https://jsonplaceholder.typicode.com/
  - https://jobs.github.com/api
  - https://github.com/public-apis/public-apis


### How does one consume/interact with a REST API
- Make a HTTP request to the URL/endpoint
- Data is sent back in the HTTP response

<br>

# HTTP Request

### Components of a HTTP request
- Endpoint (URL)
- HTTP method
  - GET (Retrieve)
  - POST (Create)
  - PUT & PATCH (Update)
  - DELETE (Delete)

- Headers, data & query parameters
  - provide addition information for the API
    - To know what to do
    - Who is the user requesting for data

### HTTP Status Codes and Error Messages
- Code 200+ (OK)
  - REST API successfully carried out

- Code 400+ (Client Error)
  - Error that originates from the client has occurred
    - Data parameters not sent in the request
    - Data parameters values not appropriate 
  
- Code 500+ (Server Error)
  - Error that originates from the Server has occurred
    - Code in the backend has error
    - Code in the backend did not account for certain edge cases
    - Code in the backend was unreachable
  
- Reference
  - <a href="https://restfulapi.net/http-status-codes/#:~:text=HTTP%20defines%20these%20standard%20status,client's%20request%20was%20accepted%20successfully.">HTTP Status Code Reference</a>

# Calling API
- Postman/Insomnia
- Python
- Javascript fetch
- show on webpage
  - document.getElementById('');
  - document.querySelector('');


querySelector is the newer feature.
getElementById is better supported than querySelector.
querySelector is better supported than getElementsByClassName.
querySelector lets you find elements with rules that can't be expressed with getElementById and getElementsByClassName



What to do next