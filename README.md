# 🎓 Project 1: Smart University Network

## Computer Networks — Complete Capstone Project

**A comprehensive solution combining a Student Management System web application with a Cisco Packet Tracer network simulation.**

---

## 📦 What's Included

This project has **two integrated components**:

### 1. 💻 Student Management System (Web Application)
- PHP + MySQL website
- 21 files, full authentication, activity logging
- Hosted on Apache server in the simulated network

### 2. 🌐 Cisco Packet Tracer Simulation
- Smart University network with Main + Branch campuses
- All 17 required networking concepts implemented
- VPN, OSPF, VoIP, QoS, and more

---

## 📁 Folder Structure

```
Project1-University-SMS/
├── 📄 README.md                  ← You are here
├── 📄 PACKET_TRACER_GUIDE.md     ← Step-by-step network build guide
├── 📄 QUICK_REFERENCE.md         ← Cheat sheet (commands & IPs)
├── 📄 PRESENTATION_SCRIPT.md     ← What to say to your professor
└── 📁 SMS-Web-App/               ← The PHP/MySQL website (21 files)
```

---

## ✅ All 17 Networking Concepts Covered

| # | Concept | Implementation |
|---|---------|----------------|
| 1 | **Subnetting (VLSM)** | 7 subnets across 2 campuses |
| 2 | **VLANs** | 7 VLANs (Admin/Staff/Students/Teachers/VoIP/Servers/Mgmt) |
| 3 | **Inter-VLAN Routing** | Router-on-a-Stick |
| 4 | **ACLs** | Block Students→Admin, restrict Teachers |
| 5 | **Routing Protocols** | OSPF Area 0 |
| 6 | **NAT/PAT** | Internet for all VLANs |
| 7 | **VPN** | IPsec Site-to-Site (Main ↔ Branch) |
| 8 | **DHCP** | 5 pools, one per user VLAN |
| 9 | **DNS** | university.edu domain |
| 10 | **STP** | Rapid PVST+ |
| 11 | **Switch Security** | Port Security with sticky MAC |
| 12 | **Static Routing** | Default route to ISP |
| 13 | **Dynamic Routing** | OSPF |
| 14 | **TCP/UDP** | HTTP (TCP) + DNS (UDP) + VoIP (UDP) |
| 15 | **VoIP** | IP Phones with Call Manager Express |
| 16 | **QoS** | Voice priority queue (40%) |
| 17 | **Network Security** | ACLs + VPN + SSH + Port Security |

---

## 🚀 Quick Start

### Setup the Web Application

1. **Install XAMPP** from https://www.apachefriends.org
2. **Copy** the `SMS-Web-App/` folder to `C:\xampp\htdocs\sms\`
3. **Start** Apache + MySQL in XAMPP Control Panel
4. **Open** `http://localhost/phpmyadmin`
5. **Import** `database.sql` → then `activity_log.sql`
6. **Open** `http://localhost/sms/login.php`
7. **Login:** `admin` / `admin123`

### Build the Network

1. **Install** Cisco Packet Tracer 8.x+
2. **Open** `PACKET_TRACER_GUIDE.md`
3. **Follow** the step-by-step instructions (~80 minutes)
4. **Save** as `University_Network.pkt`

---

## 🎯 Project Scenario

**Smart University** is a modern educational institution operating on two campuses:

### 🏫 Main Campus (Downtown)
- **Administration** (VLAN 10) — Registrar, financial offices
- **Staff** (VLAN 20) — Support staff
- **Students** (VLAN 30) — Computer labs, library
- **Teachers** (VLAN 40) — Faculty offices
- **VoIP** (VLAN 60) — IP phones across all departments
- **Servers** (VLAN 99) — SMS web server, DNS, Call Manager

### 🏛️ Branch Campus (Suburban)
- **Engineering Faculty** (VLAN 50) — Engineering department
- **VoIP** (VLAN 60) — Branch IP phones

### 🌐 How They're Connected
- Both campuses connect to the Internet via separate ISP links
- A **secure IPsec VPN tunnel** connects the two campuses
- **OSPF** dynamically advertises routes between them
- Faculty can make **VoIP calls** between campuses
- **QoS** ensures call quality even under heavy load

---

## 📊 Network Statistics

- **Total Devices:** 18
- **Routers:** 3 (Main, Branch, ISP)
- **Switches:** 4 (1× L3, 3× L2)
- **Servers:** 3 (SMS, DNS, Call Manager)
- **End Devices:** 6 PCs + 3 IP Phones
- **VLANs:** 7
- **Subnets:** 9 (with VLSM)
- **Total IPs Available:** 800+

---

## 🎓 Educational Value

This project demonstrates:

✅ **Network Design** — VLAN segmentation by department needs
✅ **VLSM Subnetting** — efficient IP space usage
✅ **Routing** — Static + Dynamic (OSPF) coexistence
✅ **Security** — Multiple layers (Layer 2, 3, 7)
✅ **Modern Services** — VoIP, VPN, QoS in one network
✅ **Real-world Application** — actual web app running on the network

---

## 💼 What You Can Demonstrate

After completing this project, you can confidently:

1. Design VLSM subnetting plans for any organization
2. Configure Inter-VLAN routing with Router-on-a-Stick
3. Set up OSPF dynamic routing
4. Configure IPsec Site-to-Site VPN
5. Deploy VoIP with Call Manager Express
6. Implement QoS policies with priority queues
7. Apply ACLs for traffic filtering
8. Enable Port Security and STP
9. Integrate web applications with network infrastructure
10. Troubleshoot using Cisco IOS commands

---

## 🐛 Troubleshooting

| Problem | Solution |
|---------|----------|
| Web app won't load | Check XAMPP Apache + MySQL are running |
| Database error | Re-import `database.sql` in phpMyAdmin |
| Cable lights red | Use Copper Straight-Through, not Crossover |
| OSPF not forming | Check `network` statements match interface IPs |
| VPN not establishing | Verify pre-shared key matches on both routers |
| VoIP phones offline | Check DHCP option 150 = Call Manager IP |
| ACL blocking too much | Use `show access-lists` to debug |

---

## 📞 Default Credentials

| Service | Username | Password |
|---------|----------|----------|
| SMS Web App | `admin` | `admin123` |
| SSH (Routers) | `admin` | `AdminPass123` |
| VPN PSK | — | `UniVPN2024` |

---

## 🏆 Why This Project Stands Out

✅ **Not just a website** — full network design + implementation
✅ **Not just a Cisco lab** — real PHP/MySQL application running
✅ **Two-layer demonstration** — application AND network engineering
✅ **All 17 concepts** — meets every requirement
✅ **Production-grade** — secure, scalable, professional

---

## 🎤 Ready to Present?

Read `PRESENTATION_SCRIPT.md` for a 10-minute demo plan that will impress your professor.

---

**Good luck with your Computer Networks project! 🚀**
