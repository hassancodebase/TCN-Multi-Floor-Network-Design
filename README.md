# TCN Multi-Floor Network Design (Cisco Packet Tracer)

## 📌 Project Overview
This project presents the design and implementation of a scalable enterprise Local Area Network (LAN) for a five-floor organization (TCN) using **Cisco Packet Tracer**.  
The network supports secure departmental segmentation, inter-VLAN communication, centralized services, and Internet access while maintaining scalability and ease of management.

The design follows **hierarchical network principles** and uses **VLANs, VLSM, trunking, DHCP, and Router-on-a-Stick** routing.

---

## 🏢 Network Requirements
- Five-floor enterprise building
- Over 100 workstations
- Department-level isolation
- Centralized routing and management
- Internal Web, DNS, and Email services
- Internet connectivity
- Scalable IP addressing

---

## 🧱 Network Architecture
**Topology:** Extended Star (Hierarchical Design)

- **Core Layer:** Router (R1) + SW-GROUND
- **Distribution Layer:** Trunk aggregation on SW-GROUND
- **Access Layer:** Floor-level switches per department

Each department operates in its own VLAN, ensuring security and performance isolation.

---

## 🧩 VLAN & Department Mapping

| Department           | VLAN ID | Subnet              |
|----------------------|--------:|---------------------|
| Sales                | 10      | 199.99.99.0/27      |
| Customer Support     | 20      | 199.99.99.96/27     |
| Hardware             | 30      | 199.99.99.160/27    |
| HR                   | 40      | 199.99.99.32/27     |
| Administration       | 50      | 199.99.99.128/28    |
| Management / Servers | 99      | 199.99.99.144/28    |

---

## 🌐 IP Addressing Strategy
- Base Network: **199.99.99.0/24**
- Subnetting Technique: **VLSM**
- Default Gateway: Router sub-interfaces
- DNS Server: Web Server (199.99.99.146)
- Address Allocation: **Router-based DHCP**

This approach minimizes address waste and allows future expansion.

---

## 🔁 Routing & Switching
- **Inter-VLAN Routing:** Router-on-a-Stick
- **Routing Type:** Static routing
- **Trunking:** IEEE 802.1Q
- **Switching:** Cisco 2960 (Layer 2)

---

## 🖥️ Servers & Services
- **Web Server:** Internal website + DNS services
- **Email Server:** SMTP and POP3-based internal email
- **Cloud-PT:** Internet connectivity simulation

All servers are hosted in the Management VLAN (VLAN 99).

---

## 🛠️ Hardware Used
- Cisco 1941 Router
- Cisco 2960 Switches
- End devices (PCs)
- Cloud-PT device
- Copper straight-through and crossover cables

---

## 🧪 Testing & Verification
- Inter-VLAN ping tests
- Server reachability
- Internet connectivity
- DHCP address assignment validation
- Email communication testing

Screenshots are available in the `screenshots/` directory.

---

## 📄 Documentation
- Full technical report: `report/`
- Packet Tracer simulation: `packet-tracer/`
- Presentation slides: `presentation/`
- Additional design notes: `docs/`

---

## ✅ Conclusion
The project demonstrates a complete enterprise LAN design that is secure, scalable, and aligned with real-world networking practices.  
It effectively integrates VLAN segmentation, efficient IP addressing, centralized routing, and automated configuration.

---

## 👤 Author
**MUHAMMAD HASSAN**  
Computer Networks Project  
