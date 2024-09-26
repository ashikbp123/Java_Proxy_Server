# Java_Proxy_Server
Overview
This project implements a simple proxy server written in Java. A proxy server acts as an intermediary between a client and the internet, forwarding client requests to the appropriate server and returning the server's response to the client. This proxy server can be used to filter, log, or modify requests and responses.

Features
Forward HTTP requests to target servers
Relay responses back to the client
Modify or log requests/responses (optional)
Multi-threaded, handling multiple client connections simultaneously
Requirements
Java Development Kit (JDK) 8 or higher
Basic understanding of Java networking (sockets, threading)
Proxy Server Structure
Main Components
ProxyServer.java

The entry point of the proxy server.
Listens for incoming connections from clients and spawns a new thread for each client.
ClientHandler.java

Handles communication between the client and the target server.
Reads the request from the client, forwards it to the target server, and sends the response back to the client.
Utilities.java (Optional)

Helper methods for logging, modifying requests, or adding headers.
