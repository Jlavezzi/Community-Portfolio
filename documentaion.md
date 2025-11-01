---



I successfully recreated my cybersecurity lab on my machine. It consists of two Kali Linux systems and two Windows operating systems. My host system runs Windows 11, while all other machines are hosted as virtual machines on this PC.  



Within the lab:  

\- The **Windows 10 VM** serves as the target machine.  

\- One **Kali Linux VM** acts as the attacker.  

\- The second **Kali Linux VM** serves as a monitoring and testing system, used to observe network traffic and host web servers for experiments.  



All the virtual machines are connected on the same subnet, with only the attacker Kali machine having internet access. The others are restricted to a localized **host‑only** network.  



I verified connectivity by pinging between the machines, and communication across the network worked successfully. Using Wireshark on the monitoring Kali, I was able to observe the network traffic in real time.  



I also performed network scanning to gather system information. Initially, I used a basic \*\*host discovery\*\* command:  

```

nmap -sn <ip\_range>

```

Then, I followed up with a more detailed (and noisier) command:  

```

nmap -A <ip\_range>

```

The detailed scan revealed more information than I expected, providing valuable insight into the network.  



---





