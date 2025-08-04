# 🛰️ Network Traffic Analysis using Wireshark and Zeek

This project demonstrates how to capture, analyze, and interpret network traffic using two powerful open-source tools: **Wireshark** and **Zeek** (formerly Bro). It is designed for cybersecurity learning, threat detection, and traffic behavior analysis in a virtual environment.

---

## 📘 Project Overview

- **Objective**: To capture and analyze live network traffic to detect suspicious patterns such as port scanning, DNS tunneling, and unusual HTTP activity.
- **Tools Used**: 
  - Wireshark – for real-time packet capture and protocol inspection.
  - Zeek – for behavior-based network traffic analysis and logging.
- **Environment**: 
  - Ubuntu 22.04 LTS (Virtual Machine using VirtualBox)
  - Sample `.pcap` files analyzed using Zeek

---

## 🛠️ Project Structure
    Network-Traffic-Analysis-Wireshark-Zeek/
├── Report/
│ ├── Project_Report.pdf
│ └── Project_Report.docx
├── Screenshots/
│ ├── wireshark_capture.png
│ ├── zeek_conn_log.png
│ └── dns_graph.png
├── Logs/
│ ├── conn.log
│ ├── dns.log
│ └── notice.log
├── Data/
│ └── sample_capture.pcap
└── Visualizations/
├── protocol_pie_chart.png
└── dns_volume_graph.png


---

## 📊 Key Features

- ✅ Real-time packet capture and filtering
- ✅ Behavioral analysis of traffic using Zeek logs
- ✅ Detection of common network anomalies
- ✅ Graphs and visualizations to represent DNS and IP traffic patterns
- ✅ Clean documentation and appendices with screenshots

---

## 🧪 How to Run This Project

⚠️ Run inside a virtual environment to avoid capturing sensitive personal traffic.

### 1. Install Wireshark and Zeek:
```bash
sudo apt update
sudo apt install wireshark zeek
2. Capture Traffic:
Open Wireshark

Select active interface (e.g., eth0)

Start capture and save it as capture.pcap

3. Analyze with Zeek:
bash
Copy code
zeek -r capture.pcap
4. Check Logs:
conn.log → connection summaries

dns.log → DNS query details

http.log → web traffic activity

notice.log → suspicious events detected by Zeek
