# wireshark-projects-2

## Detecting and Investigating Malware Traffic
# Introduction
In this project, I  use Wireshark to detect and investigate malware traffic. Identifying malicious network behavior is crucial for protecting networks and responding to security incidents.

# Skills learned
- Malware Analysis Lab Setup
- Malware Analysis
- Suspecious link Analysis
- Detecting and Analyzing malware
- Static Malware Analysis
- Dynamic Malware Analysis

# Pre-requisites
- Understanding Networking Concept
- wireshark installed in safe environment (vmaware , kali)
- Sample malware PCAP file downloaded from (https://www.malware-traffic-analysis.net/)
# Lab Setup and Tools 
- Wireshark: Download and install Wireshark from https://www.wireshark.org/download.html.
- Sample PCAP File: Download a sample PCAP file containing malware traffic for analysis.

  # Step 1
  - Open wireshark
  -  Go to "File" > "Open" and select the sample PCAP file which is downloaded.
  -  The file will load, and the captured traffic will be displayed.
    ![parrot - VMware Workstation 17 Player (Non-commercial use only) 9_1_2024 11_31_15 AM](https://github.com/user-attachments/assets/7ccf1f0e-448a-4bed-b380-c0e353323e8a)

 # step 2 :- Identified Malicious Traffic Patterns
 - Now, there is a ip addres,<172.16.1.66> have large number of ip address (note, might different in your case).
 - Let's check the resquests of this perticular ip address. Type on the filter bar <ip.addr==172.16.1.66>
 - ![parrot - VMware Workstation 17 Player (Non-commercial use only) 9_1_2024 11_56_43 AM](https://github.com/user-attachments/assets/4e58719a-b3ef-473f-8688-1bb1ec346862)
 

