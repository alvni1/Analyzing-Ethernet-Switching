<h1>Analyzing Ethernet Switching</h1>

<h2>Description</h2>
  A network is given with switches that have an empty MAC address table and PCs that have an empty ARP table. An arp table maps IP addresses to MAC addresses, this allows different PCs on a network to send data and communicate with one another. AN ARP request is generated when one PC on the network sends out a ping to another PC on the network via its CLI. The ARP request contains the destination's IP address and a request for the destination MAC address. It is sent out as a broadcast message to the other PCs on the network, but only the PC with the matching IP address will respond via a unicast message. The ARP reuqest will be forwarded by the switches on the network. The PC on the network will ping every other PC in order to populate its ARP table, making future communcation between one another fast and convenient. 

  A MAC address table is used by the switches in the network to avoid unneccsary traffic by only sending data to a specific port, instead of broadcasting and flooding all of the ports. Switches fill up their MAC address table by pinging all the PCs in the network via the CLI. 

<h2>Languages and Utilities Used</h2>

- <b>Cisco Command Line Interface</b> 

<h2>Environments Used </h2>

- <b>Cisco Packet Tracer</b>

<h2>Program walk-through:</h2>

PC1 pings each computer in the network so that it can add their MAC address to its ARP table. 
![Screenshot 2025-01-06 231707](https://github.com/user-attachments/assets/8c6e98a8-88f2-406c-aff1-7593c915d817)

![Screenshot 2025-01-06 231825](https://github.com/user-attachments/assets/43440a50-7686-422b-ae31-dc73839483c5)

The command "do show mac address-table" displays the MAC addresses after the switch pings each PC in the network. 
![Screenshot 2025-01-06 232115](https://github.com/user-attachments/assets/3aa29fd3-4a25-4040-ac75-f2246c3874d5)

The command "do clear mac address-table dynamic" clears all of the MAC addresses that were dynamically learned from the MAC address table. 
![Screenshot 2025-01-06 232229](https://github.com/user-attachments/assets/baf0351c-d30e-46c9-9bc0-ecc1d5e1a340)
