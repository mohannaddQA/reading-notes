# Socket IO

## Web Sockets

### 1- What is a Web Socket?

A WebSocket is a communication protocol that provides full-duplex communication channels over a single TCP connection. It allows for real-time, two-way communication between a client (typically a web browser) and a server, enabling efficient and persistent communication for web applications.

### 2- Describe the Web Socket request/response handshake and what happens once the connection is established.

The WebSocket handshake begins with an HTTP-based request from the client to the server. The client sends a special HTTP header called "Upgrade" with a value of "websocket" to indicate its intention to upgrade the connection.

If the server supports WebSocket, it responds with an HTTP 101 status code ("Switching Protocols") and establishes the WebSocket connection. The server also includes the "Upgrade" and "Connection" headers in its response to confirm the upgrade.

Once the WebSocket connection is established, both the client and server can send data to each other in a full-duplex manner. This means that they can send and receive messages simultaneously without the need for additional HTTP requests.

The WebSocket connection remains open until either the client or server decides to close it. This allows for continuous communication between the two parties, making WebSocket suitable for real-time applications such as chat systems, live updates, and online gaming.

### 3-Web Sockets provide a standardized way for the server to send content to a client without first receiving a \_\_\_\_ from that client.

a request

## Socket.io

### 1-What does the event handler io.on() do?

The io.on() function is responsible for listening to and handling incoming events on the server side.

When io.on() is used, it allows the server to listen for a specific event emitted by the client or other connected sockets. Once the specified event is triggered, the corresponding callback function associated with io.on() is executed, enabling the server to respond or perform certain actions based on that event.

### 2- Describe some possible proof of life or proof that the code works as expected

proof of life or proof that the code works as expected can be demonstrated by:

Successful Connection: Verify that the client can establish a connection with the server using sockets. This indicates that the basic network communication is functioning correctly.

Emit and Receive Events: Test the ability to emit events from the client and receive them on the server, or vice versa, using socket communication. This ensures that data can be transmitted between the client and server effectively.

Event Handling: Confirm that the server can handle incoming events from the client and perform the expected actions or responses. This ensures that the code is properly processing events and executing the desired functionality.

Real-Time Updates: Test the ability to send real-time updates or notifications from the server to the connected clients using sockets. This verifies that the code can push information to clients without requiring explicit requests.

### 6- What does socket.emit() do?

socket.emit() enables the transmission of custom events with data from one end of the socket connection to the other. It serves as a way to initiate communication and trigger actions between the client and server in a socket-based application.

## Socket.io vs Web Sockets

### 1- What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).

WebSocket can be likened to Git, which is a low-level version control system. It provides a protocol for real-time, bidirectional communication between a client (such as a web browser) and a server. WebSocket is a standardized communication protocol that operates at the transport layer, allowing for efficient and persistent full-duplex communication.

Socket.IO, on the other hand, is like GitHub or Auth0. It is a higher-level library built on top of WebSocket (among other transport mechanisms) that simplifies the implementation of real-time applications. Socket.IO provides additional features such as automatic reconnection, room-based communication, and built-in support for fallback mechanisms (like long polling) to ensure compatibility with a wide range of browsers.

### 2- When would you use Socket.IO?

- Chat Applications: Socket.IO's ability to establish persistent connections and enable real-time message exchange makes it well-suited for building chat applications. Users can send and receive messages instantly without the need for manual refreshing.

- Collaborative Tools: Socket.IO is ideal for collaborative tools like shared whiteboards, collaborative document editing, or real-time code collaboration platforms. It allows multiple users to interact and see each other's changes in real time.

- Real-Time Dashboards and Monitoring: Socket.IO enables live updates and real-time data visualization on dashboards or monitoring systems. It allows for instant data synchronization and enables users to see changes as they occur.

- Multiplayer Games: Socket.IO provides the necessary infrastructure for real-time interactions in multiplayer games. It allows players to communicate, synchronize game states, and update the game in real time.

- Notifications and Alerts: Socket.IO can be used to push real-time notifications and alerts to clients. It ensures that users receive immediate updates or notifications without requiring them to manually refresh their browser.

- Live Bidding or Auction Systems: Socket.IO facilitates real-time bidding and auction updates, ensuring that participants receive instant updates on bid status and price changes.

### 3- When would you use WebSockets?

WebSockets are useful in situations that require real-time, bidirectional communication between a client and a server. so the same examples as above
