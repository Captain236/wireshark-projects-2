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

 # step 2 :- Identified and Analyzed Malicious Traffic Patterns
 - Now, there is a ip addres,<172.16.1.66> have large number of ip address (note, might different in your case).
 - Let's check the resquests of this perticular ip address. Type on the filter bar <ip.addr==172.16.1.66>
 - ![parrot - VMware Workstation 17 Player (Non-commercial use only) 9_1_2024 11_56_43 AM](https://github.com/user-attachments/assets/4e58719a-b3ef-473f-8688-1bb1ec346862)
 - Now, let's check for the MAC Address of the sender... 
 -  ![parrot - VMware Workstation 17 Player (Non-commercial use only) 9_1_2024 12_12_00 PM](https://github.com/user-attachments/assets/41676148-984e-4956-81d0-ed94cf41a0a8)
 -  Now type <ip> on the filter bar to see  more details.
 -  ![parrot - VMware Workstation 17 Player (Non-commercial use only) 9_1_2024 12_30_41 PM](https://github.com/user-attachments/assets/c603646f-3412-4c34-9a9e-4f5bfbac1e4b)
 -  Now, on select one fied and go click on the frame (left side down) to see the windows Host name.
 - ![parrot - VMware Workstation 17 Player (Non-commercial use only) 9_1_2024 12_35_48 PM](https://github.com/user-attachments/assets/ff9cc102-8380-4225-a7de-da73c3c9d9c1)
 - Now, let's see the windows account user name. For this there are multiple ways like  by DHCP , HTTP etc, but i have applied kerberos filter which is use for authentication.
 - for this click on <statsics> tab , click on protocol herarchy and select kerberos protocol as a filter.
 - ![parrot - VMware Workstation 17 Player (Non-commercial use only) 9_1_2024 12_49_27 PM](https://github.com/user-attachments/assets/d0bb81c1-49b6-48aa-89f8-431258c49446)
 - ![parrot - VMware Workstation 17 Player (Non-commercial use only) 9_1_2024 12_52_19 PM](https://github.com/user-attachments/assets/cddae389-2b1c-4cf1-892f-fef627d8c6d2)
 - Select any one field and go to left side and click on cname string to see the username.
 - ![parrot - VMware Workstation 17 Player (Non-commercial use only) 9_1_2024 12_56_52 PM](https://github.com/user-attachments/assets/92143c6f-c212-4910-8e62-991c973bc059)
 - Now, click on the <file option> , then cilck on <export object> and then click on <http> to see the Attackers activity
 - ![wiershark](https://github.com/user-attachments/assets/69082b26-646a-4d4f-be52-20b52952a6a2)
 - After that we can see that the Attacker is trying to download some files, save the file and Analyze if it is malicious.
 - ![parrot - VMware Workstation 17 Player (Non-commercial use only) 9_1_2024 3_58_38 PM](https://github.com/user-attachments/assets/640d1c15-0a22-40c9-9afd-7e8ded6fe4e4)

  # Analyzing the Malicious Traffic
 - Go to the browser and type (virustotal)
 - note:- VirusTotal aggregates malware signatures collect from various antivirus engines, website scanners, file and UL analysis tools. Additionally, users can contribute to the database by submitting files, URLs, and domains.
 - click on choose file and upload the downloaded file to analyze if it is malicious or not.
 - ![parrot - VMware Workstation 17 Player (Non-commercial use only) 9_1_2024 4_22_54 PM](https://github.com/user-attachments/assets/48fb6fef-5a7f-43cb-9185-5835ef2d40e8)

 - Now, we can see that the file is malicious.
 - ![vv](https://github.com/user-attachments/assets/51e2bcfc-be05-42dc-9a10-cb0ef52a29f2)

# Documented and Reported Findings
![_C__Program Files_Notepad++_change log - Notepad++  Administrator  9_3_2024 11_02_40 PM](https://github.com/user-attachments/assets/aa857773-1f21-4b29-8203-a93d450d9324)

## Conclusion 
By completing this exercise, I have learned how to detect and investigate malware traffic using Wireshark. These skills are essential for identifying malicious network behavior, responding to security incidents, and protecting network infrastructure.









 

   



 

