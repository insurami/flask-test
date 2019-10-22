# flask-test
Flask test

## Task:
Create an API that stores relationsships between people. 

### Endpoint 1: 
Add a person (name, age, height, gender)

### Endpoint 2:
Store a relationship between two people. 

### Endpoint 3: 
If two people are connected either directly or through other relationsships. That endpoint should 
return the degree of separtion and if there is a connection. You should be able to pass either the name of the persons or their id
when checking the connection.

Example: John is connected to Mary, Mary is Connected to James, James is connected to Mike. 
Degree of seperation? connected: True, degreeOfSeperation: 3. Always return the least degree of seperation.

###  Endpoint 4:
Create an endpoint that returns how people are connected and return each persons name in the relationsship as a list. Always return the shortest path of the connection. 

Example: John is connected to Mary, Mary is Connected to James, James is connected to Mike. 
How is John connected to Mike? [John, Mary, James, Mike] 

### Things to think about:
+ Good separation of concerns. Different layers for api, business logic, data access and model
+ Testing
+ You can use an ORM but not required. We use SQLAlchemy
+ Please feel free to add other endpoints to make the API richer

### Technical requirements:
+ Python 3.6+
+ Virtual Env (I recommend pipenv)
+ Pytest
+ Flask
+ SQlite
