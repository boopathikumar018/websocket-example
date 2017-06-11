# WebSocket Example
Some examples of how to work with WebSockets.

## Simple Example

The first example just shows how to keep sessions so the server can send
messages later.

When the client opens the connection, the WebSocketEndpoint adds the session to
a list. Periodically, the MessageScheduler sends messages to all opened
sessions, while each client sends messages to the server.