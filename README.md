# Car Rental System Project Documentation

## Requirements

- Java 17
- Spring Boot
- PostgreSQL

## API Access

### Swagger

- **How to Access Swagger UI**

  - URL: `http://localhost:8080/swagger-ui.html`
  - The Swagger UI provides a graphical interface to view and test APIs.

## **PLEASE => CREATE IN THIS ORDER!**
To create the entities you can use Postman or Swagger

  to create an Agency:
  http://localhost:8080/agency/register
  {
  "name": "Agency 1",
  "address": "address",
  "type": "AGENCY",
  "password": "password",
  "status": true,
  "orders": []
  }

  to create an Automobile:
  http://localhost:8080/automobile/register
  {
  "name": "Automobile 1",
  "valuePerDay": 100,
  "year": 2000,
  "registrationNumber": "registrationNumber",
  "brand": "brand",
  "model": "model",
  "plate": "plate"
  }

to create a Customer:
http://localhost:8080/customer/register
{
"name": "Customer 1",
"address": "address",
"type": "CUSTOMER",
"status": true,
"password": "password",
"registration": "registration",
"cpf": "CPF",
"orders": [],
"employments": []
}

to create an Order:
http://localhost:8080/order/register
{
  "deliveryDate": "2024-12-12",
  "customerId": 2,
  "automobileId": 1
}

