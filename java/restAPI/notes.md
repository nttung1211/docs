## Best practice
* [RestAPI](https://github.com/nttung1211/spring-boot-microservices-best-practices)
* [Error handling mini framework](https://medium.com/the-resonant-web/spring-boot-2-0-project-structure-and-best-practices-part-2-7137bdcba7d3)

## @modelAttribute vs @requestBody
* The former is for server rendering (mostly when dealing with form or for requests encoded as x-www-form-urlencoded or multipart/form-data)
* The latter is for rest api (or for requests encoded as application/json)
* [Reference](https://stackoverflow.com/questions/43716767/spring-mvc-requestbody-vs-modelattribute)


## Error handling
### @ControllerAdvice (the newest solution of spring 4 and lower)
* [Reference](https://dzone.com/articles/best-practice-for-exception-handling-in-spring-boo)
* [@ResponseStatus](https://dzone.com/articles/spring-rest-service-exception-handling-1) (Map the Exception to the ResponseStatus)
  * ex:
    ```java
    @ResponseStatus(HttpStatus.NOT_FOUND)
    @ExceptionHandler({DogsNotFoundException.class})
    public void handle(DogsNotFoundException e) {}
    ```