# Security-Mechanisms-for-Network-Slicing-in-5G-Networks 🌐
 

## 🚀 Overview  
Design and simulate a 5G network prototype with multiple slices, each serving distinct applications. The project will implement security protocols to isolate and contain potential threats like DDoS attacks. This will demonstrate how network slicing can effectively limit the spread of attacks and enhance network resilience.

---

## 🏆 Contributors   
- **Shruti Gupta (202151151)**
- **Tridib Nandi (202151174)**
- **Dhruv Sharma (202151049)**
- **Smriti Yadav (202151159)**
- **Snehal Nalawade (202151160)**


## Mentor
**Dr. Bhupendra Kumar**

---

## ✨ Features  

### Network Topology with Slices
![image](https://github.com/user-attachments/assets/b06ce4c7-4b2b-47be-bc30-949765f994b6)

### Latency Comparison
![image](https://github.com/user-attachments/assets/2b603220-8543-4e21-8b04-1387ddf4f9f6)



---

## 📊 Observation

### Normal Conditions:
The latency under normal conditions is consistently low, with values around 5 milliseconds. This indicates the network operates efficiently in the absence of any attacks or congestion. 

### DDoS Attack Conditions:
During a DDoS attack, the latency significantly increases to approximately 55 milliseconds. This reflects the heavy congestion caused by a large volume of packets overwhelming the network, which hinders its ability to process legitimate traffic efficiently. 

### ARP Spoofing Conditions:
The latency during ARP spoofing is also elevated, close to the DDoS attack levels (~55 ms). This suggests that ARP spoofing disrupts the normal packet flow, likely due to additional delays introduced by handling spoofed ARP packets and potential rerouting or incorrect traffic targeting. 

### SYN Flood Conditions:
Similar to ARP spoofing and DDoS attacks, SYN flood attacks result in a latency spike to around 55 milliseconds. This is expected, as the attack floods the target with incomplete TCP connection requests, exhausting server resources and causing delays in handling normal traffic.

---


## Requirements

To use this project, ensure you have the following installed:

1. **Python**: Version 3.8 or higher is recommended.
2. **Libraries**:
    - `scapy`: For packet crafting and network interactions.
    - `networkx`: For creating and visualizing network graphs.
    - `matplotlib`: For plotting and visualization.
3. **Additional Tools** (if applicable):
    - Administrative/root privileges may be required for certain Scapy operations.
    - Ensure your system supports the network protocols used by this project (e.g., ARP, ICMP).

### Installation

Install the required Python libraries using:

```bash
pip install scapy
```
```bash
import networkx as nx
import matplotlib.pyplot as plt
from scapy.all import IP, ICMP, TCP, ARP, send
import time
```







## 📬 Feedback  
We welcome suggestions and improvements. Feel free to raise an issue or reach out via email- 202151151@iiitvadodara.ac.in  
