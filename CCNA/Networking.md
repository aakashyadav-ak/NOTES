## 1.IP(internet protocol)

- A unique address that identifies a device on the internet or on a local network.
- Logical address 
- An Internet Protocol (IP) address is a unique identifier assigned to each device connected to a network that uses the Internet Protocol for communication.


#####  we can change(assign) a IP dynamically/statically

**Dynamic IP:**
A dynamic IP address is assigned to a device temporarily by a Dynamic Host Configuration Protocol (DHCP) server. The address can change over time, especially when the device reconnects to the network or after a lease period expires.

ex=home networks, corporate environments

**Static IP:**
A static IP address is manually assigned to a device and does not change over time. It remains constant until it is manually changed by a network administrator.

ex=servers, network printers

### Types of IP Address

- IPv4 
- IPv6
#### IPv4 

IPv4: A 32-bit address, typically represented in decimal format as 4 octets (e.g., 192.168.1.1). It allows for approximately 4.3 billion unique addresses.

(One Octate is from 0-255)

- It has Unicast, Multicast and Broadcast style of address.
- by default it broadcast if destination is not found.

**HOST:**
 A host in IPv4 is any device assigned an IP address within a subnet, and the number of possible       hosts is determined by the host bits in the subnet mask: 2^host bits (24,16,8)-2.

##### IPv4 class

1. **Class A**
- class a= 1.0.0.0-126.255.255.255  (Number of Networks: 128 (0 to 127)
- Network bits = 8, Host bits = 24
- Number of hosts = 2^24−2=16,777,214 
- Default mask: 255.0.0.0 (/8)


