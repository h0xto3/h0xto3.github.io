---
title: Root Me FTP-Authentication Walkthrough
date: 2023-10-21 22:00:00 +0100
categories: [rootme, walkthrough]
tags: [network, ftp, ctf]
---

# Root Me FTP-Authentication Walkthrough
![FTP Stockpic](https://static2.makeuseofimages.com/wordpress/wp-content/uploads/2020/08/what-is-ftp-feature.jpg)
*Source: https://www.makeuseof.com/what-is-ftp-server/* <br> 

[FTP - Authentication](https://www.root-me.org/en/Challenges/Network/FTP-authentication)

Worth: 5 Points <br>
Level: Very Easy

## Walkthrough

First download the challenge file *ch1.pcap*. If necessary you have to allow the download explicitly. I use a Kali-Linux VM for my challenges, but you can also use Windows or macOS as long as you have [Wireshark](https://www.wireshark.org/) installed.

---
**INFO**

A .pcap (short for packet capture) file is a file format used for storing network traffic data. These files are typically generated by packet capture software and network analyzers like Wireshark, tcpdump, and others. .pcap files contain a record of network packets that were captured on a computer network. Each packet in the file includes information about the source and destination addresses, the type of packet (e.g., TCP, UDP, ICMP), the packet's payload, and various other network protocol-specific data.

---

Open the .pcap file in your desired workspace using Wireshark. It should look like this:
![Wireshark Capture Ch1](/assets/img/FTP-Ch1.png) 


Now you can filter for specific packets using the filter bar. We filter for *ftp* packets. You should easily spot the password in the listed packets:

![Wireshark Capture Ch1](/assets/img/FTP-Ch1_2.png)


**Solution: c------0**