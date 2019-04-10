# api

run from within project where api is consumed.

protoc --proto_path=..\api\proto\v1 --go_out=plugins=grpc:api/v1 ..\api\proto\v1\party.proto
protoc --plugin=protoc-gen-grpc-java --proto_path=v1 --java_out=grpc:v1 v1\publish.proto
protoc --plugin=protoc-gen-grpc-java --grpc-java_out=v1 --proto_path=v1 v1\publish.proto
 
protoc --proto_path=v1 --go_out=plugins=grpc:v1/ v1\publish.proto