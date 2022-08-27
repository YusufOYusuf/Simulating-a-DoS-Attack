<h1>Simulating a DoS Attack</h1>


<h2>Description</h2>
In this lab, I learned to simulate a DoS attack. A DoS (denial-of-service) attack is a cyber-attack in which the perpetrator seeks to make a machine or network resource unavailable to its intended users by temporarily or indefinitely disrupting the services of a host connected to the Internet.
<br />



<h2>Environments Used </h2>

- <b>Kali GNU/Linux Rolling</b> 
- <b>Terminal</b>
- <b>WireShark Network Analyzer</b>

<h2>Program walk-through:</h2>

<p align="center">
From the left sidebar click Firefox ESR and type in an address to observe network connectivity: <br/>
<img src="https://i.postimg.cc/MKJmSZ86/Screen-Shot-2022-08-26-at-6-13-51-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
<img src="https://i.postimg.cc/8z1d7y5x/Screen-Shot-2022-08-26-at-6-15-15-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
Go to the upper left part of the taskbar and click "applications" and then go to "09 - Sniffing & Spoofing" and then navigate to "WireShark" <br/>
<img src="https://i.postimg.cc/8Cf7cWhq/Screen-Shot-2022-08-26-at-6-17-11-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
  
<br />
In the Wireshark Network Analyzer window in the top bar click "capture" then click "options"  <br/>
<img src="https://i.postimg.cc/C1Vr6GJ0/Screen-Shot-2022-08-26-at-6-22-05-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
In the Wireshark - Capture Interfaces window, in the "Capture Filter for Selected Interfaces" text box type "tcp 80" and click start <br/>
<img src="https://i.postimg.cc/V6JfNcn4/Screen-Shot-2022-08-26-at-6-28-23-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
Minimize Wireshark and the open up Firefox ESR, click Open menu icon in the top right and then navigate to Library > History > Clear Recent History, make sure to chose the clear Everything options <br/>
<img src="https://i.postimg.cc/3rbG9Ktr/Screen-Shot-2022-08-26-at-6-33-13-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





<br />
Minimize the browser and open up the terminal window.  <br/>
<img src="https://i.postimg.cc/C5Dfz8kv/Screen-Shot-2022-08-26-at-6-36-18-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
In the terminal window type the following command "hping3 192.168.122.121 -p 80 -i u1000 -S -q --rand-source"  <br/>
<img src="https://i.postimg.cc/Dz9vmM6T/Screen-Shot-2022-08-26-at-6-39-07-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
Go to the Browser Window and type in the http address from before.  <br/>
<img src="https://i.postimg.cc/tgjyjx4q/Screen-Shot-2022-08-26-at-6-46-13-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />






<br />
You will observe that it will not connect to the address.  <br/>
<img src="https://i.postimg.cc/52WDYMdp/Screen-Shot-2022-08-26-at-6-48-45-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
Go back to the terminal window and hit ctrl+C to quit the attack.  <br/>
<img src="https://i.postimg.cc/yxFtnf00/Screen-Shot-2022-08-26-at-6-51-49-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />












  
  
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
