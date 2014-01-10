R_Socket
=================

R_Socket is a small c project that implements sockets, for sending messages from client side to server side.
This example may be implemented in a project for sending data from client to server, or for creating a chat program, and a lot of other stuff aswell, it all depends on your imagination.

A socket address is the combination of an IP address and a port number, much like one end of a telephone connection is the combination of a phone number and a particular extension. Based on this address, internet sockets deliver incoming data packets to the appropriate application process or thread.

An Internet socket is characterized by a unique combination of the following:
Local socket address: Local IP address and port number
Remote socket address: Only for established TCP sockets. As discussed in the client-server section below, this is necessary since a TCP server may serve several clients concurrently. The server creates one socket for each client, and these sockets share the same local socket address from the point of view of the TCP server.
Protocol: A transport protocol (e.g., TCP, UDP, raw IP, or others). TCP port 53 and UDP port 53 are consequently different, distinct sockets.
Within the operating system and the application that created a socket, a socket is referred to by a unique integer value called a socket descriptor. The operating system forwards the payload of incoming IP packets to the corresponding application by extracting the socket address information from the IP and transport protocol headers and stripping the headers from the application data.
In IETF Request for Comments, Internet Standards, in many textbooks, as well as in this article, the term socket refers to an entity that is uniquely identified by the socket number. In other textbooks,[1] the socket term refers to a local socket address, i.e. a "combination of an IP address and a port number". In the original definition of socket given in RFC 147, as it was related to the ARPA network in 1971, "the socket is specified as a 32 bit number with even sockets identifying receiving sockets and odd sockets identifying sending sockets." Today, however, socket communications are bidirectional.
On Unix-like and Microsoft Windows based operating systems the netstat command line tool may be used to list all currently established sockets and related information.

Usage
-------------
```BASH
$ gcc R_Client.c -o client
$ gcc R_Server.c - o server
```

Output Server Side
-------------
```BASH
```

Output Client Side
-------------
```BASH
```


License
--------

This code is under the BSD license.
