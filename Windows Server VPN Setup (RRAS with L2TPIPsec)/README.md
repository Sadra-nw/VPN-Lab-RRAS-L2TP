# Windows Server VPN Setup (RRAS with L2TP/IPsec)

This project documents the setup of a VPN server on **Windows Server 2022** using Routing and Remote Access Service (RRAS).  
A Windows 10 client connects to the VPN and verifies connectivity.

## Steps Documented

### 1. RRAS Dashboard  
![RRAS Dashboard](01_RRAS_dashboard.png.png)  
Routing and Remote Access successfully installed and enabled on the Windows Server 2022 machine.

### 2. Authentication and Security Settings  
![Authentication Settings](02_RRAS_authentication.png.png)  
Configured RRAS to use **Windows Authentication**.  
Enabled **L2TP/IPsec** with a **pre-shared key** for secure VPN connections.

### 3. IPv4 Address Pool Configuration  
![IPv4 Address Pool](03_RRAS_ipv4_pool.png.png)  
A static IPv4 address pool is assigned to VPN clients, ensuring proper IP allocation when connecting.

### 4. VPN Connection Established (Client-Side)  
![VPN Connected & Ping Test](04_vpn_connected_ping.png.png)  
Windows 10 client successfully connected to the VPN (`Test`).  
Connectivity verified with a **ping test** to the VPN server (192.168.248.133).

### 5. Remote Access Client Listed in RRAS  
![RRAS Client Connected](05_RRAS_client_connected.png.png)  
The connected client appears under *Remote Access Clients* in the RRAS management console.

---

## 📌 Summary
- Configured **Windows Server 2022** as a VPN server with RRAS.  
- Enabled **L2TP/IPsec** with pre-shared key authentication.  
- Created a **static IP pool** for VPN clients.  
- Verified successful connection from a Windows 10 client, including **ping tests** and RRAS session logs.  

This lab demonstrates a practical **VPN setup using RRAS** — a useful exercise for learning remote access, VPN tunneling protocols, and Windows Server administration.  
