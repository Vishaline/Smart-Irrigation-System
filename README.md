# Smart-Irrigation-System
Common for both Original and Access Point Files

1. Configure DHCP in ISP[2911 Router] by entering the following code in the CLI:
	
	conf term

	ip dhcp excluded-address 209.165.201.225 209.165.201.229

	ip dhcp pool CELL

	network 209.165.201.224 255.255.255.224

	default-router 209.165.201.225

	dns-server 10.0.0.254

	exit

	ip dhcp excluded-address 209.165.200.225 209.165.200.229

	ip dhcp pool WAN

	network 209.165.200.224 255.255.255.224

	default-router 209.165.200.225

	dns-server 10.0.0.253

	exit

3. Setup IPv4 in SmartPhone:
   
	-Desktop>>3G/4G Cell 1 Interface
	
	IPv4 Address: 172.16.1.100

	Subnet Mask: 255.255.0.0

	Default Gateway: 172.16.1.1

	DNS Server: 10.0.0.254

4. Open IoT Monitor in SmartPhone or Laptop - [Desktop>>IoT Monitor]
	In the IoT Monitor, enter:

	IoT Server Address: www.iot.org or 10.0.0.253

	UserName:admin

	Password:admin

5. All the IoT Devices can be controlled through the SmartPhone now.
   
	[This can be done by turning the IoT devices ON or OFF]

	-Conditions can be changed as required
