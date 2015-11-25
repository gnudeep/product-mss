# SimpleStockQuote Executable jar Sample

This sample demonstrates how to create an uber jar which contains your microservice as well as all its dependencies.

Here's how to deploy & run your microservice.

```java
public static void main(String[] args) {
    new MicroservicesRunner().deploy(new StockQuoteService()).start();
}
```

How to build the sample
------------------------------------------
From this directory, run

```
mvn clean install
```

How to run the sample
------------------------------------------
Use following command to run the application
```
java -jar target/stockquote-service-*.jar
```
How to test the sample
------------------------------------------

Use following cURL commands.
```
curl http://localhost:8080/stockquote/IBM

```

How to build the docker immge from the sample
------------------------------------------
From this directory, run

```
mvn clean package docker:build
```


