# Client-Server Model
- In the client-server model, a client will send a request message to a server which should respond with the data requested or a suitable message otherwise. This is commonly seen when a client browser sends an HTTP request to a web server for web page data or a web resource. The data is sent back from the server to the client's computer.
- Servers specific roles based on the data they hold and the service they provide.

### Application Programming Interfaces (API)
- An API is a set of protocols that governs how two applications should interact with one another. An API sets out the format of requests and responses between a client and a server and enables one application to make use of the service of another.
- Commonly used for gathering info. For example: Twitter's API, price comparison APIs etc.

### WebSocket Protocol
- WebSocket is a modern application layer protocol that facilitates a persistent bi-directional communication,  channel between the client and the server over a single line.
- This is known as full-duplex communication, and the packets are greatly reduced in size since they use a fraction of the usual header information.
- It also removes the need for security checks at the receiving end.
- This creates super-fast, real time and interactive communication commonly used for online gaming, instant messaging or remote document collaboration. 

### Web CRUD Applications
- Create, Read, Update, Delete are the four fundamental operations of a database or content management system.

### HTTP Request Methods
- These are equivalent to CRUD.
- Create - **Post**
- Read - **Get**
- Update - **Put**
- Delete - **Delete**

### Representational State Transfer (REST)
- REST is a style of systems design that prescribes the use of HTTP request methods to interact with online databases via a web server.
- The client required no knowledge of how the server is likely to fulfil the request.
- This allows clients and servers to operate independently of each other.
- A system or API that conforms to REST is described as being RESTful.

### Connecting To A Database Using HTTP
1. Browser makes client server request from a web server to load a web page and its resources.
2. The web page HTML file contains some JavaScript which is executed client-side.
3. The browser JavaScript calls the RESTful API which enables communication with the server-side database.
4. The database server responds to the request with data in JSON or XML format.
5. The browser renders the JSON or XML.

### JSON vs XML
- JSON and XML are the two standard methods for transferring data between the server and the web application.
- JSON uses a dictionary/list structure with simple data types.
- XML uses a HTML-like tag structure with a greater selection of datatypes.

| JSON Is:                                            | Reason:                                                                                              |
| --------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| Easier for a human to read                          | JSON code is tidier and easier to read in the data oriented format                                   |
| More compact                                        | Shorter code with fewer characters, quicker to transmit. XML fieldnames need to be written out twice |
| Easier to create                                    | Simpler syntax and structure, can also use arrays.                                                   |
| Easier for computers to parse and therefore quicker | Can be parsed by a standard JavaScript function. Numeric values are easier to differentiate from alphanumeric strings. 

### Thin vs Thick Client Computing
- The 'thickness' of a client computer refers to the level of processing and storage that it does compared to the server it is connected to. The more processing and storage the server does, the 'thinner' the client is.

| Type         | Advantages                                                                                                                                                         | Disadvantages                                                                                                                                                                                             |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Thin-client  | Easy to setup, maintain and add terminals to. Software updates can be installed automatically. More secure since data is kept centrally.                           | Reliant on the server. Requires a very powerful and expensive server. Server demand and bandwidth increased. Maintaining connection consumes more power than local processing in battery powered devices. |
| Thick-client | Robust and reliable, providing greater uptime. Can operate without a continuous connection to the server. Generally better for running more powerful applications. | More expensive, higher spec client computers needed. Installation of software required on each terminal separately. Integrity issues with distributed data.

																																					  
 
