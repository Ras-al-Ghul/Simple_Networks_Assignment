# Simple Networks Assignment  
This assignment covers basic understanding of the following topics  
1. Client-Server and Peer to Peer models.  
2. Unicast and Broadcast traffic.  
3. TCP and UDP transport protocols.  

### NOTE  
There are three directories:  
`Broadcast`, `TCP-P2P` and `ConcurrentTCP`. In general, to execute, just `make` in the respective directories and run the executable(s).  

### UDP Broadcast Program
It **broadcasts** the message `hello` and sends it through an ephemeral port. To receive this message, run the command specified in the file `command` from an other terminal/multiple terminals. `netcat` has a different behaviour. <https://stackoverflow.com/questions/7696862/strange-behavoiur-of-netcat-with-udp>  
### TCP-P2P
This takes user input for sending text messages to the other peer and also prints text messages received from the other peer. Both programs are able to send and receive messages simultaneously. Run both the executables generated within 3-5 seconds of each other, else there will be a timeout. Refer <http://cs.baylor.edu/~donahoo/practical/CSockets/>  
### ConcurrentTCP  
This TCP server can handle multiple requests coming from single/multiple clients simultaneously. While serving a request, the server doesn't block the requests coming from other clients. The server functionality is a simple echo - it echoes back the received message. Run the executable, and from an other terminal, use the command in the file `command` to connect to, and send messages to the server. Refer <http://www.microhowto.info/howto/listen_for_and_accept_tcp_connections_in_c.html>  

