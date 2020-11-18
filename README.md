# Peer-to-Peer-Network-using-Pastry-Protocol

Peer to Peer network is built using distributed programming, functional programming using F# and AKKA actor framework by implementing Pastry Protocol.

Pastry Protocol for network joining and routing in a peer-to-peer network as per the
project requirement.
- Once a new peer joins the network, the leaf-set and routing tables are
created/updated for all the appropriate nodes in the network as per the Pastry
protocol.
- Once the network is created, the application begins routing requests. Each peer
transmits numRequests requests. Requests are transmitted at the rate of 1
request/second to randomly chosen destination nodes.
- The application keeps track of the number of hops taken to reach the destination
for all the requests. The average number of hops that have to be made to deliver
the message is returned by the application.


# How to execute

  1. Run the following command
  - dotnet fsi --langversion:preview project.fsx arg1 arg2
    - arg1 is the number of nodes/peers
    - arg2 is the number of requests/files to be transferred
