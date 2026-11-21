# EXPERIMENT 4

Socket Programming for Transport Layer Packet (UDP Server)

## Terminal Session
```
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ vim udp_server_1221.c
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ gcc udp_server_1221.c -o udp_server
sit@sit-HP-ProOne-440-23-8-inch-G9-All-in-One-Desktop-PC:~$ ./udp_server
UDP Echo Server listening on port 10290...
Received from client: Hello UDP Server
Sent back to client: Hello UDP Server
```

## CONCLUSION
The UDP Server socket was successfully implemented at the Transport Layer. By utilizing `SOCK_DGRAM` with `recvfrom()` and `sendto()`, the server successfully bound to its designated port and processed incoming connectionless datagrams without establishing a prior network handshake.
