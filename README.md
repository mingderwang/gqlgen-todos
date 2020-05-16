# gqlgen-todos
test gqlgen
# run
```
go run server.go
```
then open http://localhost:8080 in a browser. here are some queries to try:
```
mutation createTodo {
  createTodo(input:{text:"todo", userId:"1"}) {
    user {
      id
    }
    text
    done
  }
}

query findTodos {
  	todos {
      text
      done
      user {
        name
      }
    }
}
```
