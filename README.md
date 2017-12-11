# grpc-gen

Create a `.grpc-gen` file such as this
```JSON
{
	"srcs_dir": "./protos",
	"srcs": [
		"example.proto"
	],
	"web_out": "./browser",
	"node_out": "./server"
}
```
And run `grpc-gen`. Stubs will be created in the folder set in `web_out` and `node_out`.

See [grpc-web](https://github.com/improbable-eng/grpc-web) on how to use the files in `web_out`. They are generated by [ts-protoc-gen](https://github.com/improbable-eng/ts-protoc-gen).

See the [gRPC Node docs](https://grpc.io/docs/tutorials/basic/node.html) on how to use the files in `node_out`. You don't need to use `grpc.load(...)`.
