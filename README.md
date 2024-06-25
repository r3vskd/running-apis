<p align="center">
<img src = 'https://github.com/r3vskd/running-apis/blob/main/images/101-postmanaut-api.png' height="320" width="400" ></img>
</p>

## APIs
 An API is an intermediate software agent that allows dependent applications to communicate with each other. APIs provide a set of protocols, 
 routines, and developer tools enabling software developers to extract and share information and let applications interact in an accessible manner.

 Be it web APIs that connect web applications to other platforms or APIs used by IoT devices to collect and process data, the use of APIs has expanded like never before.

## Types of web-based APIs
 
 ### REST-based APIs
REST (Representational State Transfer) is one of the most lucrative categories of web-based APIs. Based on Uniform Resource Identifiers (URIs) and HTTP protocol, REST-based APIs use JSON for data formatting which is considered to be browser-compatible.

 ### SOAP-based APIs
SOAP-based APIs (Simple Object Access Protocol) use a type of protocol known as Simple Object Access Protocol, which is a common communication protocol. This helps them in providing higher levels of security and makes them better at accuracy as compared with the REST-based APIs.

 ### GraphQL-based APIs
one of the most advanced sets of web-based APIs where open-source data query and manipulation language is used. This makes it easier for forming a definitive pathway for the runtime that plays a vital role in fulfilling queries with the pre-existing data.

 ### XML-RPC
XML-RPC (Extensible Markup Language-Remote Procedure Call)
Differentiates itself in terms of information security and the use of XML format that is specifically designed for transferring data. When compared to SOAP-based APIs, the XML-RPC protocols are easier and much simpler to use since they use minimum bandwidth.

 ### WebSocket
A two-way interactive communication session between the user’s browser and a server can be made smoother and faster with the help of an organized set of APIs known as WebSockets.
The entire process involving this doesn’t even require having to poll the server in order to receive a reply.

## Evolution of APIs
 <img src = 'https://github.com/r3vskd/running-apis/blob/main/images/evapis.png'></img>
  APIs interconnect individual systems that contain data about people, businesses and things, enable transactions, and create new products/services and business models. The popularity of APIs has grown significantly in the last decade or so.

## Remote procedure call (RPC) - 1981
<img src = 'https://github.com/r3vskd/running-apis/blob/main/images/rpc.png'></img>

## CORBA - 1991
 <img src = 'https://github.com/r3vskd/running-apis/blob/main/images/corba.png'></img>

 ## SOAP - 1998
  <img src = 'https://github.com/r3vskd/running-apis/blob/main/images/soap.png'></img>

## REST - 2000
  <img src = 'https://github.com/r3vskd/running-apis/blob/main/images/rest.png'></img>

## GraphQL - 2015
  <img src = 'https://github.com/r3vskd/running-apis/blob/main/images/graph.png'></img>


# Growth of the API Economy

  <img src = 'https://github.com/r3vskd/running-apis/blob/main/images/api_growth.png'></img>

# What is API Mocking?
The most common term for creating simulated components is mocking, but others are also used, and partly apply to different things; 
stubbing, simulation, and virtualization. The basic concept is the same - instead of using an actual software component (an API in our case)
– a “replacement” version of that API is created and used instead.

 - Stubbing: mostly a placeholder without real functionality
 - Mocking: basic functionality required for a specific testing or development purpose
 - Simulation: complete functionality for testing or development purposes
 - Virtualization: imulation that is deployed into an operational, manageable and controllable environment

API mocking has a number of extremely useful applications. To demonstrate this, we will use an example with a component that uses 
a number of APIs to talk to a number of auxiliary systems and services (Legacy, Mobile Apps, Infrastructure, Databases, Peer Services, 3rd Party Components):

  <img src = 'https://github.com/r3vskd/running-apis/blob/main/images/mocking.png'></img>


# CRUD operations for APIs
  Create, Read, Update, Delete—are crucial functionalities of API endpoints that need rigorous testing to ensure robust and secure interaction with a web application's back-end.

Here's a concise guide on testing CRUD operations for APIs.

  - Firstly, set up your testing environment with the necessary tools and frameworks like Postman or advanced automated testing suites if you're looking at scale.

  - Create: This will involve sending a POST request to the API with a payload that includes new resource data. Ensure that the response status code reflects
    successful creation (often a 201 code) and verify that the resource has indeed been created with all the correct attributes.

  - Read: Test the 'Read' functionality by sending a GET request. The API should return the requested resource or a collection of resources. Validate the
    correctness of the data returned and whether it meets the specification. Additionally, test for scenarios like non-existing resources or unauthorized access.

  - Update: Next, the 'Update' operation can often be the most critical. Utilizing PUT or PATCH requests, make changes to existing data and validate the success
    of these operations by checking for appropriate status codes and performing a subsequent read operation.

  - Delete: Finally, the 'Delete' operation is tested by sending a DELETE request to remove a resource. Confirm the deletion by ensuring that subsequent READ
    operations for that resource yield a 404 not found status code.

  # The First API - Django REST Framework

Django REST framework, a robust and versatile framework for creating efficient and scalable APIs. This guide is designed to provide 
you with a clear and structured approach to Django REST API, ensuring that both beginners and experienced developers can navigate 
and utilize this powerful tool with ease. 

## Step 1 -  set up a virtual envronment
```
python -m venv myenv
```
### Install Django
```
pip install django
```
### Adding Django REST Framework
```
pip install djangorestframework
```
### Verify the Installation
```
python -m django --version
```
Similarly, you can check the Django REST Framework version in your Python shell: 
```
import rest_framework
print(rest_framework.__version__)
```
