# TASK 5 – Network Traffic Capture using Wireshark

This task involves capturing and analyzing network packets using **Wireshark**, a powerful network protocol analyzer. The objective is to observe various protocols in action by generating traffic and applying filters.

---

## 🛠️ Setup Instructions

### 1. Install Wireshark

- Download from: [https://www.wireshark.org/download.html](https://www.wireshark.org/download.html)
- During installation:
  - Allow **WinPcap/Npcap** for packet capturing (essential on Windows).
- On **Linux**:
  - Search for **Wireshark** in the application manager or install via terminal.

---

## 🔄 Steps to Capture Traffic

### 2. Start Capturing on Active Network Interface

- Launch Wireshark.
- Select the **active network adapter** (e.g., Wi-Fi, Ethernet).
- Click the **blue shark fin icon** to begin the packet capture.

### 3. Generate Network Traffic

- Open a browser and visit a site, e.g., `https://google.com`
- Or run in terminal:
  '''bash
  ping google.com
  
### 4. Stop the Capture

After 30–60 seconds, click the red square icon to stop the capture.

### 5. Filter by Protocol

Use the following filters in the top filter bar of Wireshark:

tcp,
http,
dns

### 6. Identify Protocols
Look for at least three different protocols in the capture:
Protocol	Description
TCP	Reliable transport layer protocol
DNS	Resolves hostnames to IP addresses
HTTP/HTTPS	Web traffic (unencrypted/encrypted)
ICMP	Used for pings (echo requests/replies)

### 7. Save as .pcap or .pcapng
Go to File → Save As

Name your file, e.g., capture.pcap

Choose .pcap or .pcapng as format

### Output Example
Example file: capture.pcapng
