# Java TCP Socket

A simple Java TCP socket implementation demonstrating client-server communication.

## Overview

This project contains a basic TCP client-server application in Java. The server listens for incoming connections on port 5001, and the client connects to send and receive messages.

## Project Structure

```
src/
├── client/
│   └── Client.java    # TCP client implementation
└── server/
    └── Server.java    # TCP server implementation
```

## Requirements

- Java Development Kit (JDK) 8 or higher

## How to Run

### Compile the Code

```bash
javac -d out src/server/Server.java src/client/Client.java
```

### Start the Server

In one terminal, start the server:

```bash
java -cp out server.Server
```

### Run the Client

In another terminal, run the client:

```bash
java -cp out client.Client
```

## Expected Output

**Server Terminal:**
```
Hello Server..!
```

**Client Terminal:**
```
Hello Client!
```

## How It Works

1. The server creates a `ServerSocket` on port 5001 and waits for a connection
2. The client establishes a `Socket` connection to `localhost:5001`
3. The client sends a message: "Hello Server..!"
4. The server receives and prints the message, then responds with: "Hello Client!"
5. The client receives and prints the response
6. Both connections are closed

## License

This project is available for educational purposes.
