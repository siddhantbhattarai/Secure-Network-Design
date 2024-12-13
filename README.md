# **Comprehensive Network Design and Configuration**

This project is a detailed implementation of a hierarchical and secure network infrastructure for a multi-building facility. It is designed using Cisco Packet Tracer and includes configurations for VLANs, inter-VLAN routing, port security, and firewall rules.

---

## **Project Overview**
The network connects multiple buildings, including:
- Admin Building
- Manufacturing Unit
- Testing Centre
- Warehouses
- Security Booths and Amenities Building

Each section is configured with its unique VLANs, devices, and security protocols, ensuring proper segregation and communication within and across the sub-networks.

---

## **Features**
1. **VLAN Segmentation:**
   - Each department/building is assigned specific VLANs for traffic isolation.
   - VLANs configured on Layer 3 switches with IP interfaces for inter-VLAN routing.

2. **Port Security:**
   - Limits unauthorized access to the network by restricting MAC addresses on access ports.

3. **Firewall Rules:**
   - Configured to filter traffic between VLANs and external networks.
   - Ensures guest VLAN isolation from internal resources.

4. **Static Routing:**
   - Enables communication between VLANs across buildings via the Core Router.

5. **Network Address Translation (NAT):**
   - Provides internet access for internal devices while hiding private IP addresses.

6. **Scalability:**
   - The hierarchical design allows for easy expansion.

---

## **Setup Instructions**
1. **Requirements:**
   - Cisco Packet Tracer (Version 8.0 or higher).

2. **Usage:**
   - Open the `packet_tracer_file.pkt` in Cisco Packet Tracer.
   - Use the CLI on each device to view/edit configurations.

3. **Testing:**
   - Use ping tests to validate connectivity within and across VLANs.
   - Check firewall logs for unauthorized access attempts.

4. **Customization:**
   - Modify VLANs, IP ranges, or security rules as per your requirements.

---

## **Testing Procedures**
1. **Intra-VLAN Connectivity:**
   - Devices within the same VLAN should communicate successfully.

2. **Inter-VLAN Routing:**
   - Devices in different VLANs should communicate via Layer 3 switches and the Core Router.

3. **Firewall Validation:**
   - Confirm ACLs block unauthorized traffic while allowing legitimate traffic.

4. **Guest VLAN Isolation:**
   - Ensure VLAN 160 (Guest Internet) cannot access internal VLANs.

---

## **Acknowledgments**
- Cisco Packet Tracer
- OpenAI for guidance
