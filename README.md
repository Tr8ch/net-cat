# TCP Chat

TCP Chat is a simple and concurrent chat server and client written in Go, allowing users to connect and chat in real-time over a TCP network connection. It features unique usernames, chat history, and support for multiple simultaneous connections.

![TCP Chat Demo](demo.gif)

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Authors](#authors)

## Features

- Connect to the chat server using a specified host and port.
- Unique usernames for each client.
- Chat history is maintained and displayed to new clients when they join.
- Real-time chat with other connected users.
- Maximum of 10 users can connect simultaneously.

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

- [Go](https://golang.org/dl/) (Go 1.16 or later)

### Installation

1. Clone the repository:

   ```bash
        git clone https://github.com/yourusername/tcp-chat.git
   ```
2. Change into the project directory:

   ```bash
        cd tcp-chat
    ```
3. Build the server and client:

    ```bash
        go build -o TCPChat ./cmd/server
    ```
### Usage

## Starting the Server

To run the TCP Chat server, use the following command:

    ```bash
       ./TCPChat [host] [port]
    ```
 - [host] (optional): The host to bind the server to. Default is "localhost".
 - [port] (optional): The port number to listen on. Default is "8989".

## Example

Run the server on the default host and port:

    ```bash
        ./TCPChat
    ```

Run the server on a custom host and port:

    ```bash
        ./TCPChat 0.0.0.0 9999
    ```

### Connecting to the Chat

1. Connect to the server using a TCP client, such as Telnet or netcat, or use the provided TCPChatClient binary.
2. Enter your desired username when prompted.
3. Start chatting with other connected users.

### Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

Authors
[Tr8ch](https://github.com/Tr8ch)