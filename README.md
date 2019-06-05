
```bash
$ go get -u github.com/golang/groupcache
```

go run main.go -addr=:8080 -pool=http://localhost:8080,http://localhost:8081,http://localhost:8082
go run main.go -addr=:8081 -pool=http://localhost:8081,http://localhost:8082,http://localhost:8080
go run main.go -addr=:8082 -pool=http://localhost:8082,http://localhost:8080,http://localhost:8081

curl localhost:8080/color?name=red
