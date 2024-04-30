# Tutorial 9 Reflection
1. What are the key differences between unary, server streaming, and bi-directional streaming RPC (Remote Procedure Call) methods, and in what scenarios would each be most suitable? <br>

   Unary RPC typically involves a single request from a client to the server as well as a single response back from server to
client. This type of RPC would generally be used for simple operations, for example when the client sends a request yet
only expects a single response from the server. Server Streaming RPC is essentially similar with Unary RPC in which the    client would send one request, however, the server can send back multiple responses to the client. This type of RPC is     useful in cases where the server needs to send out a stream of data, responding to a single request from the client.       Finally, bi-directional streaming RPC is when both the client and server are sending out a stream of messages to one       another over a single connection. This type of RPC would be very useful in cases where both client and server require the ability to send out and receive streams of data concurrently.
   
2. What are the potential security considerations involved in implementing a gRPC service in Rust, particularly regarding authentication, authorization, and data encryption?
