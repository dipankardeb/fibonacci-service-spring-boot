#FibonacciService
A RESTful web service that:

 - Accepts a number, <code>n</code>, as input and returns the first <code>n</code> Fibonacci numbers, starting from 0.
   (i.e. given `n = 5`, the output would be the sequence "_0 1 1 2 3_")
 - The service returns the values as a String in a JSON document.
 - Given Zero or a negative number, it responds with a status code of __FORBIDDEN__ (403) and an error String in the JSON document.
 - There are unit tests that assert the algorithm output is correct.
 - The upper boundary on the input is _93_ since the _94_ value causes an overflow of a 64-bit signed value.
 - Given a value above the upper boundary, it responds with a status code of __FORBIDDEN__ (403) and an error String in the JSON document.

## Build/Deployment Instructions

This section includes the instructions necessary to build and have the web service accepting requests and responding to them.

 - Clone this [git repository]
 - Execute the following:
    - `./gradlew clean bootRun`
 - Access the endpoint(s) with a web browser or CLI tool like `curl`:
    - `curl -iv http://localhost:8080/fibonacci`
    - `curl -iv http://localhost:8080/fibonacci/0`
    - `curl -iv http://localhost:8080/fibonacci/50`
    - `curl -iv http://localhost:8080/fibonacci/100`


## JS CODE : 
run the js code like  http://localhost:8080/fibonacci/js/index.htm?n=10


