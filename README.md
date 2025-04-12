# LAN Chat App

## Overview

The LAN Chat App is a local area network (LAN) messaging application developed in C++ that allows users connected to the same network to communicate without relying on internet services. This project aims to demonstrate core networking concepts, including socket programming, multi-threading, client-server communication, and file sharing capabilities.

The application will be built using:
- **C++ Programming Language**
- **Socket Programming**
- **Networking**
- **Data Structures & Algorithms (DSA)**
- **Object-Oriented Programming (OOP)**
- **Standard Template Library (STL)**

This project does not require internet connectivity and works over a local network (LAN). Users can interact with the chat app via a simple command-line interface, send text messages, share files, and more.

## Features

- **Peer-to-Peer Communication**: The app allows users connected on the same network to send and receive messages.
- **File Sharing**: Users can send and receive files over the LAN network.
- **Client-Server Architecture**: One machine runs as the server, and others connect as clients to send and receive messages.
- **Message Encryption**: Basic encryption mechanisms to ensure secure communication.
- **Multithreading**: The server can handle multiple clients simultaneously.
- **Simple User Interface**: Text-based interface for both server and client for ease of use.

## Technologies Used

- **C++**: The primary programming language for the project.
- **Socket Programming**: For establishing communication between clients and servers.
- **Multithreading**: To manage multiple client connections simultaneously.
- **Data Structures**: To efficiently manage and process messages and files.

## System Architecture

### 1. **Client-Server Model**
   - The server listens for incoming connections and allows clients to connect to it.
   - Once a client connects, the server can receive and send messages to the client.

### 2. **Sockets and Ports**
   - The app uses sockets to establish a connection over the local area network.
   - The client connects to a predefined server IP address and port number.
   - A socket is created on both the server and client to communicate.

### 3. **Multithreading**
   - The server utilizes multithreading to handle multiple clients simultaneously.
   - Each client connection is managed by a separate thread, ensuring that one client’s actions do not block others.

### 4. **Message Encryption**
   - A simple message encryption mechanism ensures that the messages are secure.
   - Basic encryption could be added using XOR cipher or another algorithm.

## How to Run the Application

1. **Setup the Development Environment**
   - Install a C++ compiler (e.g., GCC or MinGW) to compile the project.
   - Ensure that networking libraries such as `winsock` are available for socket programming.

2. **Compile the Code**
   - To compile the code, run the following command in the terminal:

   ```bash
   g++ main.cpp network.cpp -o chatApp -lws2_32

Running the Application
<br>
Server Side: On one machine, run the server code.
./chatApp.exe

Client Side: On other machines, run the client code. Enter the IP address of the server when prompted.
./chatApp.exe


Sending Messages: Once connected, you can send text messages to the server or other clients.
File Sharing: The app also supports file sharing, where you can send and receive files between clients.


Future Enhancements
<br>
This project can be enhanced by adding the following features:
Voice/Video Chat: Integration of voice or video calling.
Message History: Store sent messages in files or databases for later retrieval.
Security: Implement stronger encryption and authentication mechanisms for secure communication.
User Authentication: Add a login system with user authentication.
GUI Interface: Develop a graphical user interface using a C++ GUI library like Qt or GTK+.
Server-Client Authentication: Secure the server-client connection with an authentication system.
Advanced File Sharing: Enable drag-and-drop file sharing, including large file transfers.

Conclusion
This LAN Chat App is a simple, effective way to communicate in a local network environment. It's a great starting point for learning about networking, socket programming, and multithreading. With further enhancements, this can become a full-fledged messaging and file-sharing application for LAN-based communication.
