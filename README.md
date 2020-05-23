This is a Spring Boot application in Java to illustrate the Hexagonal Architecture in Java.

### Relevant article:
- [Hexagonal Architecture in Java](https://medium.com/@anirban99/hexagonal-architecture-in-java-9031d3570d15)

####Build the application

1. To build the application run the command: mvn clean install 

2. To run a Spring Boot module run the command: mvn spring-boot:run

###The following REST endpoints are exposed:

####1. Retrieve all products:

curl --location --request GET 'http://localhost:8080/api/v1/product'

####2. Retrieve a specific product:

curl --location --request GET 'http://localhost:8080/api/v1/product/5'


####3. Create products: 

curl --location --request POST 'http://localhost:8080/api/v1/product' \
--header 'Content-Type: application/json' \
--data-raw '{
	"productId": 5,
    "type": "Mobile Phone",
    "description": "Apple iPhone 11"
}'

curl --location --request POST 'http://localhost:8080/api/v1/product' \
--header 'Content-Type: application/json' \
--data-raw '{
	"productId": 1,
    "type" : "Laptop",
    "description" : "Lenovo Thinkpad"
}'

####4. Remove a specific product:

curl --location --request DELETE 'http://localhost:8080/api/v1/product/5'