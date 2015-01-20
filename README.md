# jsonrpc-server 

jsonrpc-server demonstrates how to serve [Golang](http://golang.org) RPC methods over HTTP using the [JSON-RPC](http://golang.org/pkg/net/rpc/jsonrpc/) encoding. 

## Usage

### Install

```
go install github.com/kelseyhightower/jsonrpc-server
```

Start the jsonrpc server:

```
jsonrpc-server
```

### Make RPC calls using curl

```
curl -d '{"method":"Arith.Divide","params":[{"A": 10, "B":2}], "id": 0}' http://localhost:8080
```

```
{"id":0,"result":{"Quo":5,"Rem":0},"error":null}
```
