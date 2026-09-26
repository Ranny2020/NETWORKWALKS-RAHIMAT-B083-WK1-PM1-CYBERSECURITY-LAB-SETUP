# NETWORKWALKS-RAHIMAT-B083-WK1-PM1-CYBERSECURITY-LAB-SETUP

This project documents the process of setting up a personal cybersecurity laboratory using Oracle VirtualBox and Kali Linux. The challanges i faced and how it was resolved

           => Step 1. Step 1: Downloading and Installing VirtualBox
I first used the link provided in Week 1 (WK1) to download 7-Zip, which I used to extract the downloaded files. After that, I downloaded Oracle VirtualBox and extracted the necessary files. I then installed VirtualBox on my Windows computer.


            => Step 2: Configuring the Network in the VirtualBox
I configured the VirtualBox network settings to use NAT Network. I created/configured the NAT Network with the IP address 10.0.0.0/24. I also enabled the DHCP Server so that the virtual machines could automatically receive IP addresses within the network range. After making the necessary changes, I clicked Apply to save the configuration.


          => Step 3: Downloading and Setting Up Kali Linux
I used the link provided in the **PDF** to download Kali Linux. Initially, I downloaded the **Kali Linux ISO file** and attempted to install it on VirtualBox. However, I encountered difficulties and the installation was not working as expected.

                         #### Challenge Encountered and Resolution
The main challenge I faced at this stage was selecting the correct Kali Linux version for VirtualBox. Since the ISO installation was not working, I contacted one of the team leads, **Muhammad Muhammad**, who assisted me in navigating the setup and showed me the appropriate Kali Linux version to download for VirtualBox.
Following his guidance, I deleted the previous virtual machine setup and the downloaded ISO file. I then downloaded the **Kali Linux VirtualBox image** instead of the ISO file.
After downloading it, I extracted the file and opened the extracted VirtualBox file. Rather than going through the ISO installation process, the Kali Linux virtual machine started running directly in VirtualBox.
This resolved the installation issue and allowed me to successfully set up Kali Linux on my VirtualBox environment.

    => Step 4: Configuring Kali Linux Network Settings
I configured the network settings on my Kali Linux virtual machine by navigating to **Devices** and selecting **Network** in VirtualBox.
Under the network settings, I changed **Attached to** from the default option to **NAT Network**. I then selected the **NAT Network** that I had configured earlier and changed the **Promiscuous Mode** permission to **Allow All**.
After making these changes, I clicked **OK** to save the settings. This allowed my Kali Linux virtual machine to connect to the configured NAT Network.

      =>Step 5: Configuring a Static IP Address
I navigated to **Wired Connection 1**, right-clicked on it, and selected **Edit Connection**. I then clicked on **Add** and changed the connection method to **Manual**.
I configured the network settings with the following details:

* **IP Address:** 10.0.0.2
* **Netmask:** 24
* **Gateway:** 10.0.0.1
* **DNS Server:** 8.8.8.8

After applying the settings, I encountered a challenge because the network was not connecting successfully.

                   #### Challenge Encountered and Resolution
I reached out to the team lead, **Muhammad Muhammad**, for assistance. He advised me to add another IP address with the following configuration:
* **IP Address:** 10.0.0.3
* **Netmask:** 24
* **Gateway:** 10.0.0.1
After adding the new IP address and applying the changes, he also asked me to test the network connection by **pinging 8.8.8.8 from the Kali Linux terminal**. This was done to confirm that the system could successfully communicate with an external network.
After performing the ping test, the network connection was successfully established and the issue was resolved.

      => Step 6: Checking Virtual Machine Settings
I went back to the **Devices** section in VirtualBox to check the configuration of my Kali Linux virtual machine. I reviewed the available system settings and confirmed that the necessary options were enabled.
I also checked the **Acceleration** settings to ensure that the virtualization features were properly configured and functioning correctly. Everything was in order.
Finally, I checked the **Shared Folder** settings to verify the folder-sharing configuration between my Windows host system and the Kali Linux virtual machine. After confirming the settings, I was with the lab setup.



# During Week 2 of my Cybersecurity & Ethical Hacking internship,

I completed practical activities covering footprinting, reconnaissance and network scanning.In the footprinting activity, I used six Kali Linux tools to collect information about the target domain. I learned how WHOIS can provide domain information, WhatWeb can identify web technologies, Nslookup can resolve domain names, Curl can inspect HTTP headers, Wafw00f can identify a WAF, and DNSRecon can provide additional DNS information.In the network scanning activity, I used Zenmap to identify my local network configuration and discover active hosts. I also collected IP and MAC address information and created a network topology.

The exercises showed me that information gathering is an important part of cybersecurity. Even before attempting to exploit a system, a security professional can learn a significant amount about an environment by carefully analyzing publicly available information and network responses.I also learned that technical findings should be documented clearly. A good cybersecurity report should explain what was performed, what was discovered, what the observation means, what risk it may create, and what can be done to reduce that risk.
Finally, I learned that reconnaissance and scanning must always be performed within an authorized scope. 


# Week 3 Pasword Cracking With JTR / Networkwalks tools

A part of my cyber security practical training with networkwalks, i worked on a hands-on exercise focused on understanding how password-protected files can be tested.

    for the project, i :
1. downloaded and installed John The Ripper (JTR)
2. prepared a password-protected PDF for the lab
3. used the networkwalks Hash calculator to generate the PDF hash
4. Copied the hash into the password cracking tool
5. successgfully recovered the password.

This practical helped me better understand hash values, password security, and password cracking techniques.
