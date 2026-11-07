# Network Node Analyzer (Raw Socket Sniffer)

## 🇬🇧 English Description

**Network Node Analyzer** is a lightweight network traffic sniffer written in C++ using the WinSock2 API. It utilizes Raw Sockets to capture IP packets directly from the network interface, bypassing the standard transport layer.

### Features
*   Captures raw IP packets in real-time.
*   Parses IP headers (Source IP, Destination IP, Protocol, Packet Size).
*   Identifies TCP, UDP, and ICMP protocols.
*   Lightweight and console-based.

### Requirements
*   **OS:** Windows 10/11
*   **Compiler:** MSVC (Visual Studio) or MinGW (GCC)
*   **Privileges:** Must be run as **Administrator** (required for Raw Sockets).

### How to Compile
**Using MinGW (GCC):**
```bash
g++ main.cpp -o sniffer.exe -lws2_32 -liphlpapi