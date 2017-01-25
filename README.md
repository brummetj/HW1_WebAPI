# HW1_WebAPI
Postman Collection of Headers/Requests with Google Book API. 

Joshua Brummet

CSCI - 3800

Web API

01/18/17

# h2 HTTP Headers. Requests/Responses

Postman is using the HTTP requests to test the API’s for its response to get data from the calls. 
These are mainly used to test that the API is working correctly with the correct calls that the user is making. The content-type is the type of key that you are making the request with, for example, is it a authorization, or querying a string, or integers, a request can take multiple different types of headers. Using these keys will give back a response, usually in JSON, but there are multiple types of responses that come back. These responses will tell the developer whether or not that their API route has succeeded, or if there is some type of “internal error” that happened in the back-end of the web application, and or if their calls or happening correctly. The “Turing” key is a book_title variable that is queried with the API call GET /books/v1/volumes?q={{book_title}}. By creating a environment variable, the call with this variable in the request will give back the response depending what value the key has been declared. Parsing the JSON data and setting another environment variable by the JSON data from the previous API call, will allow the next GET /books/v1/volumes/{{id}}. Retrieve the response declared by the environment variable that was set. This will return the response with that variable ‘id’. 
