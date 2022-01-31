# Customer Management 
Java Backend for customer management 


## Usage 
1. POST `/api/customers/v1/` Create a customer entry 
```
http://localhost:8000/api/customers/v1/

Body 
{
	"name" : "customer1",
	"email" : "customer1@gmail.com"
}
```
2. GET `/api/customers/v1/` Get all customers
```
http://localhost:8000/api/customers/v1/

Response
[
	{
		"id": 1,
		"name": "customer1",
		"email": "customer1@gmail.com"
	},
	{
		"id": 2,
		"name": "customer2",
		"email": "customer2@gmail.com"
	}
]
```
3. GET `/api/customers/v1/{id}` Get a specific customer
```
http://localhost:8000/api/customers/v1/2

Response
{
	"id": 2,
	"name": "customer2",
	"email": "customer2@gmail.com"
}
```
4. PUT `/api/customers/v1/{id}` Update a specific customer
```
http://localhost:8000/api/customers/v1/2
Body 
{
	"name": "customer2",
	"email": "customer3@gmail.com"
}

Response
{
	"id": 2,
	"name": "customer2",
	"email": "customer3@gmail.com"
}
```
5. DELETE `/api/customers/v1/{id}` Delete a specific customer
```
http://localhost:8000/api/customers/v1/2
```