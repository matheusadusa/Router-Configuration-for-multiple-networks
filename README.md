<h1>Router Configuration for multiple networks</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
This project demonstrates how to configure a single router to handle multiple networks using Cisco Packet Tracer. It includes step-by-step visual instructions and screenshots showing how to:

- Create and connect multiple subnets
- Configure router interfaces for different networks
- Set IP addresses and subnet masks
- Enable communication between networks using routing
- Test connectivity between devices across different subnets
  
Ideal for networking students and beginners who want to understand inter-network communication and basic routing concepts in simulated environments.
<br />


<h2>Languages and Utilities Used</h2>

- Cisco Packet Tracer – for network design and simulation
- Cisco IOS CLI – for configuring router interfaces and routing via command-line
- IP Subnetting – to divide the network into multiple subnets
- Static Routing – to enable communication between networks
- Networking Concepts – addressing, subnetting, interface configuration, routing

<h2>Environments Used </h2>

- <b>macOS Ventura 13.7.4</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Launch Cisco Packet Tracer: <br/>
<img src="https://i.imgur.com/ZRUAO4Y.png"/>
<br />
<br />
Drag and drop End Devices for the 2 networks and 1 switch for each, connect the computers to its network's switch using Copper Straight-Through cables:  <br/>
<img src="https://i.imgur.com/iQ2eJ6X.png"/>
<br />
<br />
Choose a Router, drag and drop then connect both switches to it using Copper Straight-Through cables: <br/>
<img src="https://i.imgur.com/oFl1OAh.png"/>
<br />
<br />
Double click the computers, select Desktop, IP Configuration then choose Static IPV4 adresses of your choice for each computer of the 2 networks, in this case we'll use 192.168.100.1 and 192.168.100.2 for computers 1 and 2 in the left network. Then 172.16.0.1 and 172.16.0.2 for computers 3 and 4 of the right network:  <br/>
<img src="https://i.imgur.com/GxkMhMb.png"/>
<br />
<br />
On the same screen choose Default Gateways for the networks, in this case we'll use 192.168.100.254 for the left one and 172.16.255.254 for the right one :  <br/>
<img src="https://i.imgur.com/lKIvsp0.png"/>
<br />
<br />
Double click the Router, go on Config then select the port corresponding to the left network on the Interface tab, which in this case is GigabitEthernet0/0/0 and turn it on. Then on the IPV4 address field type the Default Gateway of the left network which is 192.168.100.254:  <br/>
<img src="https://i.imgur.com/hTqZVC4.png"/>
<br />
<br />
Now select the port corresponding to the right network which is GigabitEthernet0/0/1, turn it on then address the Default Gateway which is 172.16.255.254:  <br/>
<img src="https://i.imgur.com/DgnbW9T.png"/>
<br />
<br />
Done! You have succesfully configured the Router for multiple networks:  <br/>
<img src="https://i.imgur.com/ir65b3v.png"/>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
