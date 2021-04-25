## Best practice
* [refrence link](https://github.com/nttung1211/spring-boot-microservices-best-practices)

## @modelAttribute vs @requestBody
* The former is for server rendering (mostly when dealing with form or for requests encoded as x-www-form-urlencoded or multipart/form-data)
* The latter is for rest api (or for requests encoded as application/json)
* Reference: https://stackoverflow.com/questions/43716767/spring-mvc-requestbody-vs-modelattribute