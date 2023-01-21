# gRPC Web - Echo-Test

This is a full self contained working example of the grcpweb-echo example from grpc.io
It is not dependend on a big proxy which needs docker, but only uses the simple executable which is part of this repo

It even includes the correct/older version of protoc to compile javascript AND the grcp-web plugin, so no anger and worries...

## Build
`npm install`

`npm run postinstall`

`npm run make`

it will compile the proto file and compile the javascript files to be able to run in the browser
If already compiled the proto you can also just use *npm run build_client* for webpacking the javascript for the browser.

## Run

1. `npm start` this starts the grpc backend server and the proxy which will forward grpc-calls from localhost:8080 to the backend server at localhost:9090 and vice-versa
3. Run the client by opening the *echotest.html* in the browser. 

