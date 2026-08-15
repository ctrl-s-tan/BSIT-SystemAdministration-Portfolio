# T.A.N. Solutions — IT Infrastructure Plan

**Student:** Samantha E. Tan  
**Course:** BSIT 4D  
**Date:** August 15, 2026  
**Location:** CCS Building, Laguna State Polytechnic University - Santa Cruz Campus

---

## Project Overview

This project demonstrates the complete IT infrastructure planning process for a newly established startup company. As the Junior System Administrator, I was tasked with designing everything from scratch—hardware, software, networking, security policies, and documentation—before any equipment is purchased. The goal is to create a professional, scalable, and secure IT environment that supports business operations from day one.

## Learning Objectives

### Knowledge
- Explain the roles and responsibilities of a System Administrator
- Identify the hardware, software, and networking requirements of a small business
- Describe the purpose of IT documentation and infrastructure planning

### Skills
- Analyze organizational IT requirements
- Prepare professional IT inventories
- Design an enterprise network topology
- Create technical documentation using Markdown
- Present infrastructure planning professionally

### Attitude
- Professionalism
- Organization
- Technical communication
- Attention to detail
- Critical thinking

---

## Company Profile

**Company Name:** T.A.N. Solutions  
**Nature of Business:** A software development startup delivering custom web and mobile applications, internal tools, and cloud-based solutions for SMEs.

**Company Vision:** To empower businesses with reliable, secure, and scalable software that accelerates growth and operational efficiency.

**Company Mission:** To design, build, and maintain high-quality software products using modern development practices, cloud infrastructure, and strong security controls—while fostering a collaborative, learning-driven team culture.

**Office Location:** Santa Cruz, Laguna, Philippines

### Organizational Structure
- CEO/Founder
- IT Manager (oversees infrastructure and security)
- Departments: IT, Human Resources, Finance, Sales
- Junior System Administrator reports to IT Manager

### Employee Distribution

| Department | Employees |
|------------|-----------|
| Information Technology | 5 |
| Human Resources | 4 |
| Finance | 5 |
| Sales | 6 |
| **Total** | **20** |

---

## Part 2 — Enterprise Hardware Inventory

| Asset ID | Hardware | Quantity | Department / Use | Purpose & Justification |
|----------|----------|----------|------------------|-------------------------|
| HW-001 | Desktop Computers | 12 | IT (3), Finance (5), HR (2), Sales (2) | Cost-effective, stable workstations for fixed-desk roles |
| HW-002 | Laptops | 8 | IT (2), Sales (4), HR (2) | Mobility for sales and hybrid staff; IT on-site support |
| HW-003 | Server | 1 | IT (shared) | Hosts AD DS, file shares, internal apps, backup |
| HW-004 | Router | 1 | IT (network core) | Routes LAN/WAN/VLAN traffic; QoS and remote access |
| HW-005 | Switch | 1 | IT (network core) | Connects wired devices; VLAN segmentation |
| HW-006 | Network Printer | 1 | Shared (HR/Finance) | Centralized printing/scanning |
| HW-007 | UPS | 2 | Server room / network rack | Power protection and graceful shutdown |
| HW-008 | Wireless Access Point | 2 | All departments | Reliable Wi‑Fi coverage across single-floor office |
| HW-009 | NAS Storage | 1 | IT (shared) | Central file storage with redundancy |
| HW-010 | External Backup Drive | 2 | IT (backup rotation) | Offline backup copies for disaster recovery |
| HW-011 | Monitors | 14 | Desktop users + docking | Dual-monitor productivity; one spare |

---

## Part 3 — Enterprise Software Inventory

| Software | Version | License | Purpose & Why Needed |
|----------|---------|---------|----------------------|
| Windows 11 Pro | 22H2+ | Commercial | Standard OS; BitLocker, Group Policy, domain join |
| Ubuntu Server | 24.04 LTS | Open source | Stable server OS for internal services |
| Microsoft Office | Current | Subscription | Productivity suite + OneDrive/Teams |
| VS Code | Latest | Free | Primary code editor for developers |
| Git | Latest | Open source | Version control for source code |
| GitHub Desktop | Latest | Free | Git GUI for non-CLI users |
| VirtualBox | Latest | Open source | Local virtualization for testing |
| Google Chrome | Latest | Free | Standard browser for web apps |
| Microsoft Defender | Built-in + cloud | Included | Baseline antivirus/EDR |
| AnyDesk | Latest | Free/Pro | Remote support tool |
| 7-Zip | Latest | Open source | File compression for backups |
| Figma | Latest | Free/Freemium | Design tooling for startups |

---

## Part 4 — Enterprise Network Inventory

| Item | Quantity | Specification | Purpose |
|------|----------|---------------|---------|
| ISP Modem | 1 | Fiber broadband | Primary internet handoff |
| Router | 1 | Dual-WAN, VLAN, VPN | Routes traffic, enforces policies |
| Next-Gen Firewall | 1 | UTM features | Perimeter protection, segmentation |
| Switch | 1 | 24-port Gigabit, PoE+, VLAN | Connects devices, powers APs |
| Wireless Access Point | 2 | Wi‑Fi 6, PoE, WPA3-Enterprise | Secure, high-capacity Wi‑Fi |
| Patch Panel | 1 | 24-port CAT6 | Organizes cabling in rack |
| CAT6 Cables | ~30–40 runs | 1–30m assorted | Wired connections |
| RJ45 Connectors | 50+ | CAT6-rated | Patch cables and outlets |
| Spare SFP / Cables | 1 set | As needed | Future uplinks or redundancy |

---

## Part 5 — Enterprise Network Diagram

![Network Topology](ABC_Startup_Network_Topology.png)

*Figure 1: T.A.N. Solutions Office Network Topology*

### VLAN Plan

| VLAN ID | Name | Purpose |
|---------|------|---------|
| 10 | Servers & NAS | Core infrastructure |
| 20 | IT Department | IT workstations |
| 30 | HR Department | HR workstations |
| 40 | Finance Department | Finance workstations |
| 50 | Sales Department | Sales workstations |
| 99 | Guest Wi‑Fi | Visitor network (isolated) |

> **Diagram file:** `ABC_Startup_Network_Topology.drawio` (open in [draw.io](https://app.diagrams.net))

---

## Part 6 — System Administration Roles

### Helpdesk Technician
- **Responsibilities:** First-line support, IT requests, software installs, basic troubleshooting, onboarding/offboarding
- **Skills:** Communication, patience, OS familiarity, remote tools, documentation
- **Common Tools:** Ticketing system, remote tools, M365 Admin, AD user mgmt
- **Certifications:** CompTIA A+, ITIL 4 Foundation, Microsoft 365 Certified: Fundamentals

### Network Administrator
- **Responsibilities:** Design/maintain LAN/WLAN, VLANs, DHCP/DNS, firewall rules, monitoring, performance tuning
- **Skills:** TCP/IP, routing/switching, Wi‑Fi design, security basics, scripting
- **Common Tools:** Managed switches/AP controllers, firewall UI, Wireshark, NMS
- **Certifications:** CompTIA Network+, Cisco CCNA, Juniper JNCIA, Fortinet NSE 4

### Linux System Administrator
- **Responsibilities:** Install/configure Linux servers, user/permission mgmt, patching, services, backups, hardening
- **Skills:** Bash scripting, package mgmt, systemd, storage, networking, security
- **Common Tools:** SSH, rsync, cron, Ansible, Nagios/Zabbix, Git
- **Certifications:** Linux+, RHCSA/RHCE, LFCS

### Cloud Administrator
- **Responsibilities:** Provision/manage cloud resources, IAM and policies, cost monitoring, backups, security baselines
- **Skills:** Cloud platforms, IaC basics, networking in cloud, monitoring/logging
- **Common Tools:** AWS Console/CLI, Azure Portal, Terraform, CloudWatch, S3/Blob storage
- **Certifications:** AWS SysOps/Solutions Architect, Azure Administrator (AZ‑104), Google Cloud Associate

### How They Work Together
Helpdesk fixes user issues and escalates bigger problems. Network Admin keeps connections reliable and secure. Linux Admin keeps servers and core services stable and updated. Cloud Admin adds cloud capacity and enforces security policies. Together, they keep systems secure, up, and scalable.

---

## Part 7 — Infrastructure Recommendations

### Internet Provider
Choose a fiber business plan with at least 300–500 Mbps symmetric speeds and a static IP option.  
**Reason:** Supports cloud dev tools, large repos, video calls, and SaaS without bottlenecks.

### Server Specifications
- CPU: 8–12 cores
- RAM: 32–64 GB ECC
- Storage: 2×² SSD for OS/apps + 4×² HDD/SSD in RAID for data/NAS
- NIC: Dual 1GbE  
**Reason:** Handles AD, file services, internal apps, and monitoring with headroom.

### Backup Strategy (3‑2‑1)
- 3 copies of data
- 2 different media
- 1 offsite  
**Schedule:** Daily incremental, weekly full; test restores quarterly.  
**Reason:** Protects against ransomware, hardware failure, and human error.

### Security Recommendations
- Deploy NGFW with IPS, web filtering, and application control
- Enforce WPA3-Enterprise or WPA2-Enterprise with 802.1X for Wi‑Fi
- Segment networks via VLANs
- Enable endpoint protection with cloud management  
**Reason:** Reduces attack surface and contains incidents.

### Antivirus / Endpoint Protection
Use Microsoft Defender for Endpoint with cloud-delivered protection and automatic updates. Add browser isolation and controlled folder access.  
**Reason:** Strong baseline protection integrated with Windows and M365.

### Password Policy
- Minimum 12 characters; avoid common words
- Enforce MFA for all admin and cloud accounts
- Password manager company-wide; rotate only on compromise
- Lockout after 5 failed attempts; 15-minute idle timeout  
**Reason:** Balances security and usability while preventing credential attacks.

### Expansion Plan (12–24 months)
- Add second ISP line for failover at ~30 employees
- Upgrade to stackable switch or add second 24-port switch
- Introduce dedicated backup server or cloud backup service
- Formalize IT policies  
**Reason:** Ensures continuity and scalability as the startup grows.

---

## Part 8 — Personal Reflection

This project made me realize that building IT infrastructure isn't just about buying computers and plugging them in. The real work starts with understanding how the business actually operates. Once I mapped out the departments and their needs, it became easier to justify why we need specific devices, how many ports the switch should have, or why VLANs matter. I started thinking like a sysadmin: not just "what do we need?" but "why, how will it be used, and what happens if it breaks?"

The hardest part was the network diagram. I kept second-guessing myself—how many VLANs are enough, where should the firewall sit, will two access points really cover the whole office? Drawing it in Draw.io was also tricky because I had to make sure the symbols were correct, the labels were clear, and the layout wasn't a mess. It forced me to be specific about things I usually skip, like cable types, PoE requirements, and port counts.

Planning first matters because it saves money and prevents headaches. Without a plan, you end up buying the wrong gear, leaving security holes, or building a network that can't grow. A good plan lines up tech with business needs, sets standards, and gives you a realistic budget. For a startup, that's huge—every peso counts. It also gives you a reference when things go wrong, because you know what's supposed to be there and how it should behave.

This project helped me grow because I got to practice the full sysadmin workflow: gathering requirements, making inventories, designing the network, writing policies, and explaining everything clearly. I also got better at documenting my decisions, which is something I'll need in real jobs. Most of all, I now see infrastructure as something that needs constant care—documented, monitored, and improved. That "plan first, then execute" mindset is what I'll take forward in my career.

---

## References

1. Laguna State Polytechnic University. (2026). *System Administration and Maintenance Self-Paced Learning Module*. Prepared by: JOHN RANDOLF M. PENAREDONDO, MIT.
2. diagrams.net. (n.d.). *Draw.io - Free Online Diagram Editor*. https://app.diagrams.net
3. Microsoft. (2026). *Windows 11 Pro Specifications*. https://www.microsoft.com/windows
4. Canonical. (2026). *Ubuntu Server 24.04 LTS*. https://ubuntu.com/server
5. CompTIA. (2026). *Network+ and Security+ Certification Objectives*. https://www.comptia.org

---

**Prepared by:** Samantha E. Tan  
**Role:** Junior System Administrator  
**Date:** August 15, 2026  
**Course:** BSIT 4D  
**Institution:** Laguna State Polytechnic University - Santa Cruz Campus
