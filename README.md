# Multicast

Java Application that multicasts messages from a source to multiple receivers.

Program reads an input file in the format of:

7   //Number of Nodes  
5 0 10.1.1.5    //NodeNumber,  0-Source 1-Sender 2-Receiver,  IP-Address  
1 1 10.1.1.1  
2 0 10.1.1.2  
3 0 10.1.1.3  
4 2 10.1.1.4  
6 2 10.1.1.6  
7 2 10.1.1.7  
1 2 4     //Node1 Node2 WeightOfEdgeBetweenNodes  
1 3 5  
2 3 6  
2 4 4  
2 5 5  
3 5 2  
3 6 2  
4 5 5  
4 7 4  
5 7 2  
6 7 5  

Using Djikstra's Shortest Path Algorithm and Multicasting, forwards messages from the source to nodes via the shortest path.
