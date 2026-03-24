I work with an old ThinkPad with Ubuntu as OS and a VirtualBox Kali VM.

1)  
Found out there are 2 simple ways to get the Kali VM. Either the prepared File https://www.kali.org/get-kali/#kali-platforms or a walkthrough https://www.kali.org/docs/virtualization/install-virtualbox-guest-vm/.  
The Ubuntu OS for my victim computer was too old so I had to set up a brand new Ubuntu OS.

2)  
I prefered to isolate the homelab network with a hotspot from the victim, but that didn't work. So I continued in my normal home network.  
With 'ip a' on both systems I looked up for the ip address and pinged with 'ping VICTIM_IP' to see if a connection is possible.
Next step was to install OWASP Juice Shop on the victim. The Kali System could now see with 'nmap -sV VICTIM_IP' that there was an open port on 3000.
