# RESTful API Example with golang
This is simple example restful api server only with **gorilla/mux**.  
For simplifying code, this example uses a mock database that is `map[string]interface{}`

## Install and Run
```shell
$ go get github.com/kkamdooong/go-restful-api-example

$ cd $GOPATH/src/github.com/kkamdooong/go-restful-api-example
$ go build
$ ./go-restful-api-example
```

## API Endpoint
- http://localhost:3000/api/v1/companies
    - `GET`: get list of companies
    - `POST`: create company
- http://localhost:3000/api/v1/companies/{name}
    - `GET`: get company
    - `PUT`: update company
    - `DELETE`: remove company

## Data Structure
```json
{
  "name": "golang",
  "tel": "012-345-6789",
  "email": "golang-nuts@googlegroups.com"
}
```