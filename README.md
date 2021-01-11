# go-project-1

A RESTful API example for simple application with Go

It is a just simple tutorial or example for making simple RESTful API with Go and PostgreSQL.

## Pre-requests 
1. PostgreSQL with a username: "postgres" and password: "" running on port: 5432
2. Golang
3. A database named 'testdb' with the table structure:
 ```SQL
 CREATE TABLE COMPANY(
  ID INT PRIMARY KEY     NOT NULL,
  NAME           TEXT    NOT NULL,
  AGE            INT     NOT NULL,
  ADDRESS        CHAR(50),
  SALARY         REAL
);
```

## Build and Run
```bash
git clone https://github.com/yashptel/go-project-1.git
cd go-project-1
go run main.go

# API Endpoint : http://127.0.0.1:8080/
```

## Structure
```
└── main.go
```

## API

#### /company
* `POST`: Add an employee detail

#### /company/{id}
* `GET` : Get an employee detail
* `PUT` : Update an employee detail
* `DELETE` : Delete an employee detail

## Todo

- [x] Support basic REST APIs.
- [ ] Get all employee details with a single GET request.

