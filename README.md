# wex-test-upstream

Place to store service contract `proto` and generated gRPC service code.

## To generate gRPC service code

```bash
# generate proto message & custom type
protoc -I=./proto --go_out=./svc ./proto/purchaseService.proto

# generate rpc methods & service client
protoc -I=./proto --go-grpc_out=./svc ./proto/purchaseService.proto
```