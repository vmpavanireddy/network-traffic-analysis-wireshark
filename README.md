# Network Traffic Analysis using Wireshark

This guide explains how to capture and analyze network traffic using Wireshark, a powerful open-source packet analyzer.


## Step-by-Step Instructions

### 1. Install Wireshark
Download Wireshark from the official website:  
[https://www.wireshark.org/download.html](https://www.wireshark.org/download.html)

Install using default settings.  
*Note:* On Windows, Npcap will also be installed to enable packet capturing.


### 2. Select the Network Interface
- Open Wireshark.
- You'll see a list of available network interfaces (e.g., Wi-Fi, Ethernet).
- Select the active interface (such as Wi-Fi).
- Click the **Start Capturing Packets** button (shark fin icon).


### 3. Start Capturing Traffic
- Wireshark will begin displaying live network traffic.
- Optionally, perform activities like browsing a website or transferring files to generate traffic.


### 4. Apply Display Filters
Focus on specific traffic by applying filters such as:

- `http` — Show only HTTP traffic.
- `tcp.port == 80` — Show traffic on port 80.
- `ip.addr == 192.168.1.1` — Filter traffic to or from a specific IP.
- `dns` — Show DNS queries.


### 5. Analyze Packets
- Click on individual packets to see detailed information.
- Wireshark has three panes:
  - **Packet List Pane** (top)
  - **Packet Details Pane** (middle)
  - **Packet Bytes Pane** (bottom)


### 6. Follow Streams
- Right-click a packet → **Follow** → **TCP Stream** or **UDP Stream**.
- This helps analyze complete conversations, such as HTTP requests and responses.


### 7. Identify Suspicious Traffic (Security Analysis)
Look for:

- Unknown or unfamiliar IP addresses.
- Unusual ports (other than common ones like 80 or 443).
- High-frequency traffic possibly indicating DoS attacks.
- Unencrypted sensitive information (e.g., plaintext credentials).


### 8. Save or Export the Capture
- Go to **File → Save As** to save your capture as a `.pcap` file.
- Use this for offline analysis or for sharing reports.


### 9. Generate Statistics
Use the **Statistics** menu for insights:

- Protocol Hierarchy
- Conversations
- Endpoints
- IO Graphs (to visualize traffic over time)


### 10. Stop Capturing
Click the red square **Stop** button to end the packet capture.


## Author

Pavani  
VIT-AP University  

