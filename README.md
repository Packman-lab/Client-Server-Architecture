# Client-server-architecture using opengl

### OBJECTIVES OF THE PROJECT :

•	To implement the concepts of computer graphics. 

•	To design an interactive demo of working of client-server model. 

•	Simulation of data transmission between client and server using TCP. 

•	Simulation of data transmission between client and server using UDP. 

•	Simulation of data transmission from one client to another using server as a centralized system. 


### DESIGN :

The entire project is itself designed in C++ using Visual Studio. The simulation is performed by considering 1 server in the center and 4 clients around it. The server is centralized i.e. all the communications among the clients has to be done through the server itself. 

Client 1 makes use of TCP to transmit data to the server. Similar to HTTP, the client first sends a client request to the server and the server responds with the server response. The Client, after receiving the server response can again transmit the data (if any) to the server and similarly, the server also can transmit the data to the client. Client request and response are demonstrated using animating lines.  
Client 2 makes use of UDP to transmit data to the server. In this case, there is no need of handshaking. Instead, the data is directly pushed towards the server and vice versa. In UDP, there is no method to detect packet loss. In this case datagram packet transmission is shown using animating lines.  
Client 3 and Client 4 demonstrate how data is transmitted among these 2 clients through the central server. First one client (say client 3) uploads some data to the server (that is not present in the server). If the same data is required by another client (say client 4), they download it from the server itself. 
Notice that client to client data transmission is not possible without the influence of server.  
