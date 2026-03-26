# Zabbix Monitoring Lab

## 📌 Overview
This project demonstrates a monitoring environment built using Zabbix to simulate real-world NOC (Network Operations Center) scenarios. 

The lab focuses on detecting, analyzing, and resolving issues across multiple layers including:
- Network (ICMP)
- Services (SSH)
- System performance (CPU)
- Monitoring infrastructure (Zabbix agent)

---

## 🧱 Architecture

Zabbix Server (Ubuntu)
│
├── Ubuntu Server (Zabbix Agent)
└── (Planned) Windows Host

---

## ⚙️ Technologies Used

- Zabbix (Monitoring Platform)
- Ubuntu Linux
- KVM Virtualization
- Wireshark (for future packet analysis)
- GNS3 (planned for network simulation)
- VyOS (planned for routing scenarios)

---

## 🚨 Monitoring Features Implemented

- ICMP-based host availability monitoring
- SSH service monitoring using TCP checks
- CPU and system performance monitoring
- Zabbix agent health monitoring
- Trigger dependency configuration for alert suppression

---

## 🧠 Key Concepts Practiced

- Root cause analysis vs symptom alerts
- Layered monitoring (network vs service vs host)
- Alert correlation using trigger dependencies
- Performance vs outage troubleshooting
- Monitoring blind spot identification

---

## 🧪 Scenarios Simulated

### 1. Network Failure
- Disabled network interface
- Observed multiple alerts
- Identified ICMP as root cause
- Verified dependency suppression of SSH and agent alerts

---

### 2. SSH Service Failure
- Stopped SSH service
- Verified host remained reachable
- Confirmed service-level alert only

---

### 3. Zabbix Agent Failure
- Stopped Zabbix agent
- Observed monitoring gap
- Distinguished between monitoring issue and system issue

---

### 4. High CPU Utilization
- Generated load using stress tool
- Monitored CPU metrics
- Identified top resource-consuming processes
- Practiced performance troubleshooting

---

### 5. Monitoring Blind Spot
- Simulated service failure without proper monitoring
- Identified lack of alert coverage
- Implemented additional service checks

---

## 🔧 Tools Used for Troubleshooting

- ping (connectivity validation)
- nc / netcat (port checks)
- systemctl (service management)
- top / htop (performance analysis)
- ss (port listening verification)

---

## 🚀 Future Improvements

- Add Windows host monitoring
- Integrate network topology using GNS3
- Implement SNMP monitoring for network devices
- Configure alerting (email/Slack)
- Build dashboards for visualization

---

## 💡 Key Takeaway

This project demonstrates the ability to:
- Build monitoring systems
- Simulate real-world failures
- Perform structured troubleshooting
- Identify root causes instead of reacting to symptoms

---
