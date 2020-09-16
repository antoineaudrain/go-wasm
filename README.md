# go-wasm

Let's learn [Golang](https://golang.org/) and [Web Assembly](https://webassembly.org/)!!!

## Setup

build main.wasm from main.go :

```
GOOS=js GOARCH=wasm go build -o main.wasm
```

start server usind goexec :

```
goexec 'http.ListenAndServe(`:8080`, http.FileServer(http.Dir(`.`)))'
```
