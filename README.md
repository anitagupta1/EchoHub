# EchoHub(Multi-Client Chat Application)

This is a multi-client chat application developed in C++ using socket programming. 


## Features
- **Multi-client support**: Enables multiple users to join the chat room.
- **Color-coded messages**: Each client has a unique color, making chat easier to follow.
- **Graceful exit**: Clients can safely exit the chat with `Ctrl+C`, and other clients are notified of their departure.
- **Threaded message handling**: Uses separate threads for each client to enable real-time message exchange without blocking.

## Project Structure
- **`client.cpp`**: Contains the client-side code for connecting to the server, sending and receiving messages, and handling the user interface.
- **`server.cpp`**: Contains the server-side code for managing client connections, broadcasting messages to all clients.

## Requirements
- **C++ compiler** (GCC or another compatible compiler)
- **Linux or Unix-based environment** (the application is built and tested on Linux)
- **Basic terminal knowledge** to compile and run C++ files

## How to Set Up and Run the Application

### Step 1: Clone the Repository
Clone this repository to your local machine or download the files manually.

```bash
git clone https://github.com/yourusername/multi-client-chat-application.git
cd multi-client-chat-application
```

### Step 2: Compile the Server and Client Programs
Clone this repository to your local machine or download the files manually.

```bash
g++ server.cpp -o server -lpthread

g++ client.cpp -o client -lpthread
```
### Step 3: Start Server
```bash

./server
```

### Step 3: Start Client
```bash

./client
```
