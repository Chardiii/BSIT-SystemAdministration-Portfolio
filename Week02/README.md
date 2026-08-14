# Enterprise IT Infrastructure Plan — ABC Startup Solutions
**Course Module:** System Administration and Maintenance  
**Academic Institution:** Laguna State Polytechnic University (LSPU)  
**Instructor:** John Randolf M. Penaredondo, MIT  
**Portfolio Folder:** `BSIT-SystemAdministration-Portfolio/Week02/`

---

## 1. Project Overview
This project presents a comprehensive, ground-up IT Infrastructure Plan for **ABC Startup Solutions**, a newly established software development company with 20 employees on a single office floor. The project covers enterprise hardware and software provisioning, network design and topology, local ISP and server recommendations (Laguna, Philippines context), security policies, and administrative role mapping.

---

## 2. Learning Objectives
* Design a complete enterprise IT infrastructure from scratch for a small-to-medium enterprise (SME).
* Formulate detailed hardware and software inventories aligned with specific departmental job roles.
* Create a scalable and secure enterprise network topology using standard networking symbols.
* Recommend reliable infrastructure solutions (ISP, backup strategy, security policies) tailored to local operational environments.
* Practice professional documentation and version control workflows using Git and GitHub.

---

## 3. Company Scenario
* **Company Name:** ABC Startup Solutions
* **Nature of Business:** Software Development
* **Location:** Laguna, Philippines (Single Office Floor)
* **Total Workforce:** 20 Employees
  * **Information Technology:** 5 (Developers / SysAdmins)
  * **Human Resources:** 4
  * **Finance:** 5
  * **Sales:** 6
* **Initial State:** Greenfield deployment (no existing computers, servers, network, cabling, or security policies).

---

## 4. Hardware Inventory Summary

| Asset ID | Equipment | Qty | Department | Key Role |
| :--- | :--- | :---: | :--- | :--- |
| `HW-DESK-01` | Desktop Workstations (Core i5, 16GB RAM) | 9 | HR (4), Finance (5) | Stationary, secure data processing |
| `HW-LAPT-01` | High-Performance Laptops (Core i7, 32GB RAM) | 5 | IT (5) | Code compilation, mobile virtualization |
| `HW-LAPT-02` | Standard Business Laptops (Core i5, 16GB RAM) | 6 | Sales (6) | Client demos, mobility, presentations |
| `HW-SERV-01` | 1U Rackmount Server (Xeon, 64GB RAM, RAID 5) | 1 | IT / Central | Active Directory, DNS/DHCP, Staging |
| `HW-ROUT-01` | Enterprise Gigabit Router | 1 | IT / Central | LAN/WAN edge routing, VPN gateway |
| `HW-FIRE-01` | Next-Generation Hardware Firewall (NGFW) | 1 | IT / Central | Deep packet inspection, security rules |
| `HW-SWIT-01` | 24-Port Gigabit PoE+ Managed Switch | 1 | IT / Central | Workstation connectivity, AP PoE power |
| `HW-WAP-01` | Wi-Fi 6 Dual-Band Access Points | 2 | IT / Central | Seamless office wireless coverage |
| `HW-NAS-01` | 4-Bay NAS Storage (RAID 5) | 1 | IT / Central | Centralized storage, snapshot backups |
| `HW-BACK-01` | External Backup Drives (8TB) | 2 | IT | Air-gapped weekly off-site rotation |
| `HW-UPS-01` | Double-Conversion Online UPS | 2 | IT / Server Room | Clean power and battery failover |
| `HW-PRIN-01` | Enterprise Multi-Function Network Printer | 1 | HR / Finance / Admin | Shared physical documentation |
| `HW-MONI-01` | 27-inch LED Displays | 20 | All Employees | Workstation display & productivity |

---

## 5. Software Inventory Summary

| Software | Version | License | Primary Function |
| :--- | :--- | :--- | :--- |
| **Windows 11 Pro** | 23H2 | Commercial / OEM | Endpoint OS (BitLocker & AD integration) |
| **Ubuntu Server** | 24.04 LTS | Open Source (GPL) | Server OS (Hosting internal services) |
| **Microsoft 365 Apps** | Latest | Commercial Subscription | Standard corporate office suite |
| **Visual Studio Code** | Latest Stable | Freeware (MIT) | Primary development IDE |
| **Git & GitHub Desktop** | Latest Stable | Open Source / Freeware | Distributed version control & GUI |
| **VirtualBox** | 7.0+ | Open Source (GPLv2) | Local sandbox and mobile emulation |
| **Microsoft Defender** | Integrated | Included with OS | Centralized endpoint protection (EDR) |
| **AnyDesk** | Latest Stable | Commercial License | Remote administrative troubleshooting |
| **7-Zip** | Latest Stable | Open Source (LGPL) | Secure file compression & archiving |

---

## 6. Enterprise Network Diagram

The network topology follows a defense-in-depth architecture:  
`Internet (ISP Modem) → Edge Router → Next-Gen Firewall → 24-Port Core Managed Switch → VLAN-Segmented Workstations & Wireless APs`.


---

## 7. Technologies Used
* **Network Design & Modeling:** Draw.io
* **Documentation & Markdown:** Visual Studio Code, GitHub Flavored Markdown (GFM)
* **Version Control:** Git, GitHub Desktop
* **Operating Systems Planned:** Windows 11 Pro, Ubuntu Server 24.04 LTS
* **Infrastructure Concepts:** VLAN Segmentation, RAID 5, 3-2-1 Backup Strategy, NIST Password Guidelines

---

## 8. Challenges Encountered
1. **Accurate Hardware Sizing:** Determining the right balance between processing performance for the IT team and budget-conscious hardware for HR and Finance.
2. **Network Port Allocation:** Calculating exact physical port requirements (including wall drops, server uplinks, NAS, and PoE for access points) to fit within a single 24-port managed switch.
3. **Local Environmental Planning:** Factoring in the power grid reliability in Laguna, which necessitated specifying double-conversion online UPS units to protect server hardware against power fluctuations.

---

## 9. Reflection
Planning this infrastructure project highlighted the critical role that early preparation plays in enterprise IT. Designing systems from scratch requires thinking beyond just individual computer specs—it demands an understanding of workflow requirements, data security, network segregation, and business continuity. This module reinforced essential system administration fundamentals and developed the practical problem-solving skills needed for real-world IT deployments.

---

## 10. References
* Bureau of Labor Statistics, U.S. Department of Labor. (2025). *Computer Support Specialists*. Occupational Outlook Handbook. https://www.bls.gov/ooh/computer-and-information-technology/computer-support-specialists.htm
* Bureau of Labor Statistics, U.S. Department of Labor. (2025). *Network and Computer Systems Administrators*. Occupational Outlook Handbook. https://www.bls.gov/ooh/computer-and-information-technology/network-and-computer-systems-administrators.htm
* CompTIA. (2024). *What Is a Linux Administrator?* CompTIA IT Career News. https://www.comptia.org/en-us/blog/your-next-move-linux-administrator/
* Koenig Solutions. (2023). *Microsoft Azure Administrator Roles and Responsibilities*. https://www.koenig-solutions.com/blog/microsoft-azure-administrator-roles-and-responsibilities
* Koenig Solutions. (2023). *Red Hat System Administrator Roles and Responsibilities, Job Description & Salary*. https://www.koenig-solutions.com/blog/red-hat-system-administrator-roles-and-responsibilities-job-description-salary
