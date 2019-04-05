# api

run from within project where api is consumed.

protoc --proto_path=..\api\proto\v1 --go_out=plugins=grpc:api/v1 ..\api\proto\v1\party.proto