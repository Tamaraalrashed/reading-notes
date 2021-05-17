# Express

### The difference between PUT and PATCH

In a PUT request, the enclosed entity is considered to be a modified version of the resource stored on the origin server, and the client is requesting that the stored version be replaced.

With PATCH, however, the enclosed entity contains a set of instructions describing how a resource currently residing on the origin server should be modified to produce a new version.

Also, another difference is that when you want to update a resource with PUT request, you have to send the full payload as the request whereas with PATCH, you only send the parameters which you want to update.

>I got the answer from [DevQA](https://devqa.io/difference-put-patch-requests/)


## Services or tools that allow you to “mock” an API for development 

1. *[Postman](https://www.postman.com/).*
2. *[Mocky.io](https://designer.mocky.io/).*
3. *[MockServer](https://www.mock-server.com/).*

##  Swagger and APIDoc HTTP status codes should be sent with each type of (un)successful API call

 ***For Docapi:***
```
@apiErrorExample Error-Response:
 *     HTTP/1.1 404 Not Found
 *     {
 *       "error": "UserNotFound"
 *     }
 or:
 * @apiError   401/Unauthorized          Invalid basic auth credentials supplied.
 or:
 * @apiError   403/Forbidden             Required field [...] omitted.
 ```

 ***For Swagger:***
 ```
 400:
          description: Bad request. User ID must be an integer and bigger than 0.
        401:
          description: Authorization information is missing or invalid.
        404:
          description: A user with the specified ID was not found.
```

## SOAP and REST
SOAP (Simple Object Access Protocol) is a standards-based web services access protocol that has been around for a long time. Originally developed by Microsoft.

REST (Representational State Transfer) is another standard, made in response to SOAP’s shortcomings. It seeks to fix the problems with SOAP and provide a simpler method of accessing web services. 

***The Similarities***
While SOAP and REST share similarities over the HTTP protocol, SOAP is a more rigid set of messaging patterns than REST. The rules in SOAP are important because we can’t achieve any level of standardization without them. REST as an architecture style does not require processing and is naturally more flexible. Both SOAP and REST rely on well-established rules that everyone has agreed to abide by in the interest of exchanging information.


***Differences:***
1. for SOAP :Language, platform, and transport independent (REST requires use of HTTP).
2. for SOAP :Works well in distributed enterprise environments (REST assumes direct point-to-point communication).
3. REST is more efficient (SOAP uses XML for all messages, REST can use smaller message formats).
4. REST is faster (no extensive processing required).
5. REST is closer to other web technologies in design philosophy.
6. SOAP has built-in error handling.

## Node
It is an open-source, cross-platform runtime environment that allows developers to create all kinds of server-side tools and applications in JavaScript. The runtime is intended for use outside of a browser context (i.e. running directly on a computer or server OS). As such, the environment omits browser-specific JavaScript APIs and adds support for more traditional OS APIs including HTTP and file system libraries.

## Express

The most popular Node web framework, and is the underlying library for a number of other popular Node web frameworks.<br>
While Express itself is fairly minimalist, developers have created compatible middleware packages to address almost any web development problem. There are libraries to work with cookies, sessions, user logins, URL parameters, POST data, security headers, and many more. 

## NPM

npm is the world's largest software registry. Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to manage private development as well.

npm consists of three distinct components:

- the website: it's the website for [npmjs](https://www.npmjs.com/), which used for  discovering packages, set up profiles, and manage other aspects of your npm experience
- the Command Line Interface (CLI) :runs from a terminal, and is how most developers interact with npm.
- the registry : it is a large public database of JavaScript software and the meta-information surrounding it.


## TDD

Test-driven development” refers to a style of programming in which three activities are tightly interwoven: coding, testing (in the form of writing unit tests) and design (in the form of refactoring). <br>


It has a set of rules:

- write a “single” unit test describing an aspect of the program.
- run the test, which should fail because the program lacks that feature.
- write “just enough” code, the simplest possible, to make the test pass.
- “refactor” the code until it conforms to the simplicity criteria.
- repeat, “accumulating” unit tests over time.<br>

Why we Use TDD:
- “code coverage” is a common approach to evidencing the use of TDD; while high coverage does not guarantee appropriate use of TDD, coverage below 80% is likely to indicate deficiencies in a team’s mastery of TDD.
- version control logs should show that test code is checked in each time product code is checked in, in roughly comparable amounts.


## CD and CI

Continuous integration(CI) is a coding philosophy and set of practices that drive development teams to implement small changes and check in code to version control repositories frequently. Because most modern applications require developing code in different platforms and tools, the team needs a mechanism to integrate and validate its changes.


Continuous delivery picks up where continuous integration ends. CD automates the delivery of applications to selected infrastructure environments. Most teams work with multiple environments other than the production, such as development and testing environments, and CD ensures there is an automated way to push code changes to them.

CI/CD tools help store the environment-specific parameters that must be packaged with each delivery. CI/CD automation then performs any necessary service calls to web servers, databases, and other services that may need to be restarted or follow other procedures when applications are deployed.