# Snort Config

<h2>Description</h2>
In this network security task, I installed and configured snort, explored different sniffing modes curling to google, and logging the sniffed packets in the current directory.   


<h2>Languages and Utilities Used</h2>

- <b>snort</b>
- <b>linux CLI</b>


<h2>Environments Used </h2>

- <b>Unbuntu</b> 

<br />
<br />
Installed snort.

![1) installed snort](https://github.com/user-attachments/assets/f061edea-f34b-4cc6-bd34-fe09a8af18a3)

<br />
<br />
First domain queried and assocaited ip address. 

![2) backing up snort config](https://github.com/user-attachments/assets/596b5ed3-dd6d-428d-9040-55baccc8a4b9)

<br />
<br />  
Backed up snort.conf with snort.conf.bak. 

![4) scroll down to custome rules and comment out default rules](https://github.com/user-attachments/assets/87b4de10-4c4d-430f-8b03-1ae1c86d61f6)
<br />
<br />
Tested snort to validate the config with the command line below. 

![5) validating snort after commenting out all rules](https://github.com/user-attachments/assets/2a661e67-3ec4-4b5d-a671-ed5b7dfaaf04)

<br />
<br />
Ran snort to sniff -i enp0s3 and curled google.com.

![6)curl google and sniffed packets](https://github.com/user-attachments/assets/93a06e9f-7183-4b3b-99d9-bdbbc2508d7a)

<br />
<br />
Ran sudo snort -i enp0s3 -e to sniff a curl to google.com. -e enables snort to display the data link layer packet headers in its output with more detailed information about each packet, including MAC addresses and other link-layer details.

![7) -e to see more headers](https://github.com/user-attachments/assets/765b834b-5cb7-4314-9a5b-7c7c62d871ee)

<br />
<br />  
Running sudo snort -i enp0s3 -d while curling to http://example.com to show us the payload output in HEX & ASCII format with -d. 

![8) sudo snort -i enp0s3 -d shows ASCII ](https://github.com/user-attachments/assets/f69d350e-fb0a-45c0-8157-71d8de6bb9f2)

<br />
<br />
Ran sudo snort -i enp0s3 -l. to log the snort sniff into the current directory (-l.).

![9) sudo snort -i enp0s3 -l  to log to current directory](https://github.com/user-attachments/assets/5d8cef03-2c0d-4665-b410-6933f1137628)

<br />
<br />
