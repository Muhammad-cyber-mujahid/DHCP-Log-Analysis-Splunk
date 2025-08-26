<img width="955" height="423" alt="DHCP_SERVER" src="https://github.com/user-attachments/assets/9928a978-8185-464c-9d90-21481d5b1d8a" /><img width="958" height="430" alt="Broadcast_Request" src="https://github.com/user-attachments/assets/9e3e53a7-59d7-459a-a823-e416dc6a57db" /><img width="938" height="468" alt="Succesful-IP-Assignments" src="https://github.com/user-attachments/assets/2a5cc3d2-4532-486b-bb68-ba71adf2eec1" />This contains the insights derived from the DHCP logs

- List All DHCP Transactions
<img width="947" height="470" alt="DHCP-ALL-EVENTS" src="https://github.com/user-attachments/assets/c4d46d05-d412-4a4b-8ae4-247ff5a8a6c9" />

This splunk query shows every device’s MAC address, requested IP address, assigned IP address, lease duration and timestamp. It provides us with a full picture of DHCP activity

-  Top Devices by Request Count
<img width="956" height="404" alt="Top-Device-Request" src="https://github.com/user-attachments/assets/f20cea5c-823a-44c8-a4f2-9b80d32007b6" />

This identifies the device with the most request by counting how many times each MAC requests an IP, further highlighting potentially busy or misconfigured devices

Failed IP Assignments with Duration=0
<img width="958" height="463" alt="Failed-IP-Assignments" src="https://github.com/user-attachments/assets/ba42eb93-46c5-4d4d-a4fe-28f0cdc57eff" />

This lists devices failing to get an IP lease, pointing to network errors or potential probing.


Successful IP Assignments with Duration>0
<img width="938" height="468" alt="Succesful-IP-Assignments" src="https://github.com/user-attachments/assets/70039b48-e033-45e5-bc4c-0fae42c07027" />

This shows devices successfully assigned IPs with their lease durations that is 86400 seconds = 24 hours, indicating normal network behavior.

Broadcast Requests
<img width="958" height="430" alt="Broadcast_Request" src="https://github.com/user-attachments/assets/8c7fe98c-7542-4498-bc4d-def7c26d8372" />

This Identifies devices sending DHCP discovery requests and it's usefulness can be found in understanding network join attempts or spotting excessive scans.

Request Frequency Over Time
<img width="959" height="304" alt="Request-Frequency-Over-Time" src="https://github.com/user-attachments/assets/764fea27-0a8b-494f-941c-50b0671175ea" />

This tracks how often devices request IPs in 10-minute windows, highlighting spikes that could indicate abnormal activity.

DHCP Server Interactions to specific DHCP server
<img width="955" height="423" alt="DHCP_SERVER" src="https://github.com/user-attachments/assets/0e155516-8ec3-4925-9660-e01246000ad1" />

This shows how devices interact with a DHCP server (192.168.202.1), revealing server load and lease patterns.






