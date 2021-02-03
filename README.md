# WebAPI2RPC

## Intro:
A lightweight highly abstracted extension that creates a gRPC web API from a normal .NET API controller. This gRPC API will hook into existing controllers rather than services.

## Requirements:
1.	Non-breaking addition to existing .Net web API’s
2.	Ability to run both the REST and gRPC versions of the API at the same time
3.	gRPC API code should be abstracted out of sight unless the dev wants to see it for debugging reasons then a build variable can be used
4.	Transcodes API at build/compile time
5.	Conversion from HTTP status codes to gRPC status codes where possible

## Optional extras:
1.	Swashbuckle integration

## Useful links
* The reverse of what I would like to do (gRPC --> REST) https://github.com/aspnet/AspLabs/tree/master/src/GrpcHttpApi
* gRPC IO state of gRPC web - https://grpc.io/blog/state-of-grpc-web/
* gRPC for .NET - https://github.com/grpc/grpc-dotnet
* gRPC gateway https://github.com/grpc-ecosystem/grpc-gateway. This is the standard for felxability between REST and gRPC as it allows the front end to hit the gateway as HTTP 1.x and pass JSON but the backend can consome it as a protocol buffer
