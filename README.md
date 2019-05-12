# api

#### Run from within project where api is consumed
``` protoc --proto_path=..\api\v1\proto --go_out=plugins=grpc:api/v1 ..\api\v1\proto\party.proto ```
