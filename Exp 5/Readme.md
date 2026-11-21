# EXPERIMENT 5

Socket Programming for Transport Layer Protocol (UDP Client)


## Terminal Session
```
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ vim udp_client_1221.c
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ gcc udp_client_1221.c -o udp_client
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ ./udp_client 127.0.0.1
Enter message to send: Hello UDP Server
Echo from server: Hello UDP Server
```

## CONCLUSION
The UDP Client socket was successfully implemented at the Transport Layer. Using connectionless datagram sockets (`SOCK_DGRAM`) along with `sendto()` and `recvfrom()`, the client successfully transmitted and received packets from the server without requiring a dedicated connection circuit or prior handshake.
