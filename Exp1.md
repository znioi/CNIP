# Experiment 1: Introduction to Network Simulator (Packet Tracer) and Establishing a Peer-to-Peer Network

## Aim:
The objective of this experiment is to introduce the use of Cisco Packet Tracer to simulate network devices and establish a peer-to-peer network connection between two PCs. This exercise will help in understanding how to create a simple network topology, assign IP addresses, observe data flow, and analyze the network traffic between hosts.

## Theory:
A peer-to-peer (P2P) network allows two or more computers (peers) to communicate directly with each other without the need for a centralized server. In this experiment, we will use Cisco Packet Tracer, a powerful network simulation tool, to build a basic network topology and simulate data communication between two PCs.

## Steps to Download Cisco Packet Tracer:
1. Visit the official Cisco Networking Academy website: [Cisco Packet Tracer Download](https://www.netacad.com/courses/packet-tracer).
2. Create a free Cisco Networking Academy account if you do not already have one.
3. Once logged in, navigate to the "Resources" section, and download the Packet Tracer installer compatible with your operating system.
4. Follow the installation instructions to set up Cisco Packet Tracer on your system.

## Packet Tracer Interface:
After opening Cisco Packet Tracer, you will see the following main areas:
1. **Toolbar**: Contains tools for selecting devices, connecting cables, and configuring network devices.
2. **Device Selection Panel**: Shows available devices such as PCs, routers, switches, and more.
3. **Workspace**: Where you design your network topology by dragging and dropping devices.
4. **Device Configuration Panel**: Allows you to configure and view settings for selected devices.
5. **Command Prompt**: You can access the command line interface (CLI) for advanced device configuration.

## Steps to Create a Topology:
1. **Launch Packet Tracer**: Open Cisco Packet Tracer to start a new project.
2. **Add Devices**: Drag and drop two "PC" devices from the device panel onto the workspace.
3. **Connect Devices**:
   - Select the "Connections" tool (represented by a lightning bolt icon).
   - Choose "Copper Straight-Through" cable to connect the PCs to each other. Attach one end of the cable to the "FastEthernet" port on one PC and the other end to the "FastEthernet" port on the second PC.
4. **Assign IP Addresses**:
   - Click on each PC, go to the "Desktop" tab, and select "IP Configuration."
   - Assign IP addresses in the same subnet (e.g., PC1: 192.168.1.1 and PC2: 192.168.1.2 with a subnet mask of 255.255.255.0).
5. **Verify the Connection**: Use the "Command Prompt" on both PCs to test the connectivity by pinging the other PC’s IP address.

## Exercise:

### 1. Design a Peer-to-Peer Network:
- Create a simple topology with two PCs connected directly via Ethernet cables.
- Assign IP addresses (e.g., PC1: 192.168.1.1, PC2: 192.168.1.2) and subnet mask (255.255.255.0) to each PC.
- Verify the physical connection and IP configuration.

### 2. Observe the Flow of Data from Host to Host:
- Create network traffic by sending a ping from one PC to the other.
- Observe the transmission of packets by watching the communication process in Packet Tracer.

### 3. Check Functionality and Outputs in the Command Prompt:
- Open the Command Prompt on both PCs.
- Use the **ping** command to test connectivity between the PCs.
  - Example command: `ping 192.168.1.2` (on PC1).
  - Verify successful responses to ensure the PCs are communicating properly.

## Conclusion:
In this experiment, you have successfully created a simple peer-to-peer network using Cisco Packet Tracer. You have assigned IP addresses to two PCs, established a direct connection, and verified the flow of data using ping. This exercise helped in understanding basic networking concepts and how to simulate them using a network simulator.

## References:
- Cisco Networking Academy: [https://www.netacad.com](https://www.netacad.com)
- Cisco Packet Tracer Documentation: [https://www.netacad.com/course/packet-tracer](https://www.netacad.com/course/packet-tracer)

---


### 1. **What is a peer-to-peer network?**
   **Answer:**  
   A **peer-to-peer (P2P)** network is a type of network topology where two or more computers (peers) communicate directly with each other without relying on a centralized server. Each device on a P2P network can act as both a client and a server, meaning they can both provide and consume services. In this experiment, we created a simple P2P network by connecting two PCs together and allowing them to communicate by assigning IP addresses.

### 2. **Why do we assign IP addresses to the devices in a network?**
   **Answer:**  
   IP addresses are used to uniquely identify devices in a network, ensuring that data sent over the network reaches the correct destination. In a peer-to-peer network, assigning IP addresses enables each device (PC) to identify each other and facilitate communication. The IP address acts as the device's "address" within the network, allowing data to be routed properly between the devices.

### 3. **How did you configure the IP addresses for the two PCs in Packet Tracer?**
   **Answer:**  
   To configure the IP addresses in Packet Tracer:
   1. Click on the first PC, go to the **Desktop** tab, and then select **IP Configuration**.
   2. In the IP Configuration window, set the **IP address** to `192.168.1.1` and the **Subnet mask** to `255.255.255.0`.
   3. For the second PC, follow the same steps, but assign the IP address `192.168.1.2` and use the same subnet mask `255.255.255.0`.
   The devices are now in the same network range, allowing them to communicate directly.

### 4. **What is the significance of the subnet mask?**
   **Answer:**  
   The subnet mask defines the size of the network and determines which part of the IP address is used to identify the network and which part identifies the host. For example, a subnet mask of `255.255.255.0` indicates that the first three octets (192.168.1) represent the network, and the last octet (the 1 in `192.168.1.1`) identifies the specific device (host) within that network. This allows devices within the same network to communicate with each other, as they share the same network portion in their IP addresses.

### 5. **What steps did you take to physically connect the two PCs in Packet Tracer?**
   **Answer:**  
   To connect the two PCs in Packet Tracer:
   1. I selected the **Connections** tool (represented by a lightning bolt icon).
   2. I then chose the **Copper Straight-Through** cable, which is typically used for connecting devices like PCs to switches or directly to other PCs.
   3. I connected one end of the cable to the **FastEthernet** port of the first PC and the other end to the **FastEthernet** port of the second PC.
   This physically connected the two PCs in the simulation.

### 6. **How did you test the network connectivity between the two PCs?**
   **Answer:**  
   To test the network connectivity between the two PCs, I used the **ping** command in the **Command Prompt** on both PCs:
   1. On PC1, I opened the Command Prompt and typed `ping 192.168.1.2` (the IP address of PC2).
   2. If the connection was successful, I would see a series of reply messages indicating that packets were successfully transmitted from PC1 to PC2 and vice versa.
   If the ping test was successful, it meant that the two PCs were correctly connected and could communicate with each other.

### 7. **What would you do if the ping test failed?**
   **Answer:**  
   If the ping test failed, I would troubleshoot by:
   1. **Checking the IP configuration**: Ensuring that both PCs have IP addresses in the same subnet (e.g., `192.168.1.1` and `192.168.1.2` with the subnet mask `255.255.255.0`).
   2. **Checking the physical connection**: Verifying that the cable is correctly connected between the two PCs and the proper port is being used.
   3. **Testing for network device issues**: If there are additional network devices (such as routers or switches), make sure they are correctly configured.
   4. **Verifying Firewall settings**: On some operating systems, firewalls might block ping requests, so I would check if the firewall is causing the issue.
   
   After performing these checks, I would reattempt the ping test.

### 8. **Explain how you observed the flow of data between the two PCs.**
   **Answer:**  
   In Packet Tracer, I used the **Simulation Mode** to observe the flow of data. Simulation mode allows you to see the transmission of packets between devices step by step. Once I initiated the **ping** command, I could watch the packets being generated by one PC and sent across the network, arriving at the second PC. This feature is helpful for understanding the underlying process of packet transmission and how data moves through a network.

### 9. **What is the role of the Command Prompt in testing network functionality?**
   **Answer:**  
   The **Command Prompt** is a tool that allows network administrators to run various commands, such as **ping**, **ipconfig**, and others, to test and diagnose network connectivity. In this experiment, the **ping** command was used to test the connectivity between the two PCs. The Command Prompt provides a simple and effective way to troubleshoot network issues by displaying results like response times and packet loss.

### 10. **Why did you use a copper straight-through cable to connect the two PCs?**
   **Answer:**  
   A **copper straight-through cable** is typically used to connect different types of devices, such as a PC to a switch or two PCs directly. It connects the transmitting pins on one device to the receiving pins on another. In this experiment, we used the straight-through cable to connect two PCs directly. Although in real-world setups, this would typically be done with a switch, in this simplified experiment, the direct connection works because the PCs are configured to communicate on the same network.

### 11. **What would happen if you connected the two PCs using a crossover cable?**
   **Answer:**  
   A **crossover cable** is used to directly connect two similar devices, such as two PCs or two switches, without the need for an intermediary device like a hub or switch. However, in Packet Tracer, Cisco devices typically handle both straight-through and crossover cables automatically, so either cable could work for connecting two PCs. In a real-world scenario, a crossover cable would be preferred for directly connecting two PCs without using a switch.

---
