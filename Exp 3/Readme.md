# EXPERIMENT 3

Socket Programming for Transport Layer Packets (TCP Client)

## Terminal Session
```
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ vim client_1221.c
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ gcc client_1221.c -o client
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ ./client 127.0.0.1
Connected to server. Enter message: Hello Server
Echo from server: Hello Server
```

## CONCLUSION
The TCP Client socket was successfully constructed at the Transport Layer. Using the active open mechanism (socket, setting server parameters, and connect), the client successfully established a connection with the server via the TCP Three-Way Handshake and enabled reliable stream-based data transmission.
