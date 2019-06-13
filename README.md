# RestAssured API test automation

This project has automated tests for sample open source apis.

### Modules

* no modules in this project

### Tech

This project uses a number of open source projects to work properly:

* Java
* TestNG
* Slf4j
* Lombok

### How to run this project

Checkout the project from gitlab using following command
```sh
$ git clone https://github.com/shirishameka/rest-assured.git
```

Get in-to the project folder

```sh
$ cd rest-assured
```

To build the project and run the tests
```sh
$ mvn clean install
```

To only run the tests
```sh
$ mvn clean test
```

### Reading Logs

Tests write logs while they are running which provide further information about what happened if case of failure.
These files reside in ./logs directory and can be viewed locally in your browser by navigating to that folder.

### Sample Automation suite

### SpaceX API Docs:

Description
This collection of documents describes the resources and functions that make up the r/SpaceX API.
The most current version of the API is v3, with the following base URL - https://api.spacexdata.com/v3
One of the API endpoints is  /launches/past. This endpoint returns all the launches made by SpaceX till date. This endpoint allows us to sort the launches by date range by providing 2 query params - start and end(both are mandatory for sorting).


### API Details
Sample Request URL: https://api.spacexdata.com/v3/launches/past?start=2017-06-22&end=2017-06-25

Expected:
In response, every launch object has rocket details. Rocket has 2 stages - the first stage is core and the second stage is the payload. Core and payload objects have details whether this component was re-used or not. You need to print the following.
1. Mission name
2. Rocket name
3. core_serial (only if the core is reused)
4. payload_id (only if the payload is reused)

