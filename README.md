# TP1_Sec_Reseaux
![LOGO](https://user-images.githubusercontent.com/99618982/225015198-317d743a-74b9-44ad-a13b-7e698620b346.jpeg)
Realisé Par : Adil Erraad

# Sommaire:

 1. **Introduction:**
 
    1. *Objectifs de ce TP :*
    
    2. *Outils logiciels :*
    
 2. **Network Topology:**
 
 3. **Access List:**
 
 4. **Conclusion:**
 
 
 
### 1. Introduction:

*In this report, we will discuss the practical exercises or TP that we completed using Packet Tracer, a network simulation tool. The objective of this TP was to gain practical experience in tracing a network and configuring an access list. We learned how to use the Packet Tracer interface to design, configure, and troubleshoot virtual networks, and how to configure access lists to control network traffic. The skills we acquired in this TP are essential for many careers in IT and networking, and this report will highlight our experience and the lessons we learned.* 

   1. *Objectifs de ce TP :*
   >
   > - Familiarizing yourself with the Packet Tracer interface.
           
   > - Tracing the topology of a given network.
           
   > - Configuring and testing an access list on a router or other network device.
           
   >
   
   2. *Outils logiciels :*
   >
   > Cisco Packet Tracer
   >
   
### 2. Network Topology:
 
 *So What is topology*
 
 topology refers to the physical or logical layout of a network, including the arrangement of its devices, connections, and communication paths. In a physical sense, network topology describes how devices are physically connected to each other, such as through cables or wireless signals
 
 In this applied work, we have to draw this topology using the Packet Tracer tool and make it work
 
 ![2023-03-14 19_26_50-tp1 - Paint](https://user-images.githubusercontent.com/99618982/225102657-8f7c6df8-36ea-4437-b4a6-a6ff3ff93ccd.jpg)


Before starting, we must know what tools in topology and what kind of them we will use.

> we've got:

> 3 Routers : PT-Routers

> 4 Switches: 2960(type of Switch)

> 8 Computers:PC

Now let's start the settings:

- Open the Packet tracer tool and put the outils:

We will start by placing the computers and then specifying an IP address for each computer


![tp1-2](https://user-images.githubusercontent.com/99618982/225105386-36f04e45-6343-4447-974d-d6470e582b7a.png)

And to add an IP address to the computer, you must:

 - Double click in the Computer:

![2023-03-14 19_40_34-PC0](https://user-images.githubusercontent.com/99618982/225105993-2e4b3dbc-df34-4756-8a0e-195638d61f8a.jpg)

- Click in Ip Configuration And put th ip address for each laptop with his passerile(We will use it later):


![2023-03-14 19_45_40-PC0](https://user-images.githubusercontent.com/99618982/225106715-4db8e502-fe8c-4304-bb4f-165effcacd68.jpg)


- Now we have:

![TP1-3](https://user-images.githubusercontent.com/99618982/225105505-b793f9a1-eb2c-457a-897a-77fa6fe9ed8c.png)

- Now is the Time for make link between the laptop by -> Switch

![TP1-4](https://user-images.githubusercontent.com/99618982/225107298-e8dbeb13-e17c-435a-968f-d21ffa2cde7c.png)

- let's change the name of Switch by Double click and go into CLI(Command line interface)

![TP1-5](https://user-images.githubusercontent.com/99618982/225107546-6e94d91b-c116-423b-91f6-119c4010b911.png)

- Now link each Switch with his laptop using The Copper Straight Cable:

![TP1-6](https://user-images.githubusercontent.com/99618982/225107869-1bc84f71-38d8-4ecd-abf9-3ee02e3ae4ce.png)

- Let's check the connection between PC0 and PC1 by using the command prompt:

![TP1-7](https://user-images.githubusercontent.com/99618982/225108199-e54ae466-ae43-4b71-bbfe-8178914a03c5.png)

- Now will add the routers tomake the topology linked and using serial DTE cable for link between the routers:

![TP1-8](https://user-images.githubusercontent.com/99618982/225108404-314ca67e-6bb7-4fa9-ad29-28fbb7fbf8c1.png)

- as you can see we have link the network but he did'nt work  Because the port is not activated Let's Activate

- First need to go to the router and go into CLI

![TP1-9](https://user-images.githubusercontent.com/99618982/225108986-6ba88c95-f776-4679-a77b-fbadad9b5c06.png)

- Now the port active for transfer the data 

![TP1-10](https://user-images.githubusercontent.com/99618982/225109346-4e158942-ba04-4f62-84b5-b4eb3ac974cd.png)

- But we need first to give the ip address for each port of Routers

![TP1-11](https://user-images.githubusercontent.com/99618982/225109524-87bcb6e2-3835-44d3-b3dd-4cf14d8c88e9.png)

![TP1-12](https://user-images.githubusercontent.com/99618982/225109556-5baa1923-296f-4717-b3f9-eb1fa9cd15ef.png)

- In this addresse we have the passerel of the previous laptop so the connection between laptop linked by the same router will work without any problem.

![TP1-14](https://user-images.githubusercontent.com/99618982/225109928-6b850dab-6ce6-4025-a90d-ba8095a2002c.png)

- Let's Check it :

![TP1-15](https://user-images.githubusercontent.com/99618982/225110184-afad82d7-2ab9-4056-aae5-77470d8f4b2c.png)

- For make the connection work with laptop in different networks we need to enable the port forwarding for each router :

- This For the first Router we do the same things but by different configuration for thr fourwarding

![TP1-16](https://user-images.githubusercontent.com/99618982/225110533-ed15abb3-7513-4729-a98d-ddf415418146.png)

![2023-03-14 20_06_19-R1](https://user-images.githubusercontent.com/99618982/225111542-c384c8c6-872c-436b-a43f-e4bec0e23d0f.jpg)

- Let's check by using the first laptop (PC0)

![TP1-17](https://user-images.githubusercontent.com/99618982/225111719-60ebffd3-8e4e-4204-8b83-9cee837e38cd.png)

- As u can see we have connection with successful between laptopn in different networks

![TP1-19](https://user-images.githubusercontent.com/99618982/225112357-b43f9804-cc29-4152-b8d8-527d829471dd.png)

- Now we finish the part Network Topology by create the topology using the Bucket tool and make the network operational

![TP1-18](https://user-images.githubusercontent.com/99618982/225113190-f62f8e46-ccdd-4b8e-adbb-0ccfa1cf39e0.png)

### 3. Access list:

*we will discuss the practical exercises we completed to apply an access list in a network using Packet Tracer. An access list is a set of rules that determines which network traffic is allowed or denied based on specific criteria, such as the source and destination IP addresses, ports, or protocols. By applying an access list, we can control the flow of network traffic and improve network security.*

- In order to show how they work and how to use them, we will do some scenarios:

1- Allow packets sent from machine 200.4.1.2 and deny from machine 200.4.1.3 go to network 200.4.3.0:

- for this we need to create a access-list for deny any packet come from the machine 200.4.1.3 into 200.4.3.0 and let any other packets to pass

![TP1-22](https://user-images.githubusercontent.com/99618982/225116339-b0c520cf-78d0-4ee2-9c18-83a4f0297661.png)

- as u can see block the packet of 200.4.1.3 into 200.4.3.0 and allow the others , Let's check!

 PC0
 
![TP1-23](https://user-images.githubusercontent.com/99618982/225116549-8414c888-9156-4496-b78a-3a7cf765ab34.png)

PC1 

![TP1-24](https://user-images.githubusercontent.com/99618982/225116620-6c1c83da-0332-48bc-8385-04c2aee59543.png)

-its's work

2- Reject packets coming from machine 200.4.3.3 and go to 200.4.2.0 and 200.4.1.0:

- for do this 










