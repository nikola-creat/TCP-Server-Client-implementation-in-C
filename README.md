# TCP-Server-Client-implementation-in-C

Prerequisites – Socket Programming in C/C++, TCP and UDP server using select, UDP Server-Client implementation in C 

If we are creating a connection between client and server using TCP then it has a few functionalities like, TCP is suited for applications that require high reliability, and transmission time is relatively less critical. It is used by other protocols like HTTP, HTTPs, FTP, SMTP, Telnet. TCP rearranges data packets in the order specified. There is absolute guarantee that the data transferred remains intact and arrives in the same order in which it was sent. TCP does Flow Control and requires three packets to set up a socket connection before any user data can be sent. TCP handles reliability and congestion control. It also does error checking and error recovery. Erroneous packets are retransmitted from the source to the destination.

The entire process can be broken down into the following steps:

<img src='Socket_server-1.png'/>

The entire process can be broken down into following steps:

TCP Server – 

using create(), Create TCP socket.
using bind(), Bind the socket to server address.
using listen(), put the server socket in a passive mode, where it waits for the client to approach the server to make a connection
using accept(), At this point, connection is established between client and server, and they are ready to transfer data.
Go back to Step 3.
