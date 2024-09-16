<h2>Description</h2>
This is a beginner-friendly guide to downloading, installing, and using Wireshark for basic network traffic analysis. This tutorial covers step-by-step instructions and tips. Additionally, Wireshark is a free and open-source program used to capture and analyze network traffic. Furthermore, this program allows you to see data being sent and received across a network in real-time. Wireshark is often used by network administrators, security professionals, and developers to troubleshoot issues, monitor network performance, and analyze potential security threats. This program is almost like a "magnifying glass" for understanding what is happening behind the scenes when devices communicate over the internet or within a local network.
<br />

<h2>Applications Used </h2>

- <b> <a href="https://www.wireshark.org/">Wireshark</b> </a> 

<h2> Tutorial Portion</h2>

<p align="center">
Go to the Wireshark's webpage to download the application. For ease of use, I added a hyperlink to the webpage in this tutorial. Next, Select the appropriate download link for your computer.<br />
<img src="https://i.imgur.com/Nb7J7qz.png" height="80%" width="80%" alt="Wireshark's webpage."/>
<img src="https://i.imgur.com/zNL4xG5.png" height="80%" width="80%" alt="Choosing the right download link."/>

<p align="center">
Once the program finishes downloading, run the program, click <b>noted</b> on the license aggreement and make sure you have <b>Install Npcap</b> checked in the installasion wizard. Additionally, if you already have Npcap installed in your system and want to update it, you must uninstall it before downloading wireshark. If your version is the same, you can just leave the option unchecked. If you had checked <b>Install Npcap</b>, the Npcap installation wizard will pop up and just click next and install the program. <br />
<img src="https://i.imgur.com/pluQQao.png" height="80%" width="80%" alt="Wireshark installation wizard."/>
<img src="https://i.imgur.com/gPV1nDH.png" height="80%" width="80%" alt="Npcap Option in the installation wizard."/>

<p align="center">Once opening Wireshark, you will see all the interfaces your system has available to choose from. Within the <b>Enter a capture filter ...</b> field, you are able to specify which type of packets you want to capture. For example you can specify which port to use, such as <code>port 80</code>, which will only capture HTTP packets or <code>tcp</code> to only show TCP packets. Within the <b>Apply a display filter....</b>, you can filter through the packets, but will capture all the packets which match the capture filters. This option is different from the capture filters. The blue shark fin is what you will press to start the packet capture, when done you will press the square which will turn red during the packet capture to show where to click when done capturing packets. <br />
<img src="https://i.imgur.com/ikIT0sq.png" height="80%" width="80%" alt="Wireshark interface list to choose from."/>
<img src="https://i.imgur.com/GK9U90q.png" height="80%" width="80%" alt="Adding capture filters to Wireshark."/>
<img src="https://i.imgur.com/tnD4Wo3.png" height="80%" width="80%" alt="Showing the packet capture fin."/>

<p align="center">To open a packet capture (any <code>.pcap</code> file, <a href="https://archive.wrccdc.org/pcaps/">Click here for some sample files</a>.), which you may need to do is go to file, then open or <code>Ctrl+O</code>. Then go to the file where the <code>.pcap</code> file is located. Once you open the packet capture, you will notice that the program changes and shows all the packet captures within that file, starting with the first one, which is shown in the first column (No.). The (Time) column show when the packet was captured when starting the packet capture. The (source) and (Destination) columns shows the packet's IP source and Destination address respectively. The (Protocol) column shows what type of packets they are such as <code>HTTP, TCP, UDP, DNS, ARP</code>.The (Length) shows you the amount of bytes within each packet. Lastly the (info) column is just a quick description of each packet, for example a TCP packet's info column will indicate if it is a <code>SYN or ACK</code> packet. In the packet details pane, which is the bottom portion of the Wireshark program, shows each the structure of each and every packet. Formated into 'layers' where you can see from the Network layer to the Application layer. In this example, you can see the <code>HTTP</code> (Hypertext Transfer Protocol) layer showing that the packet requested to connect to <code>microsoft.com</code> <br />
<img src="https://i.imgur.com/MbsuqWn.png" height="80%" width="80%" alt="Opening a packet capture."/>
<img src="https://i.imgur.com/8qBjwuQ.png" height="80%" width="80%" alt="Chooseing the file to capture."/>
<img src="https://i.imgur.com/kklaEuB.png" height="80%" width="80%" alt="How it shows when opening the packet capture."/>
<img src="https://i.imgur.com/K3tZa7r.png" height="80%" width="80%" alt="Showing the bottom portion of Wireshark."/>