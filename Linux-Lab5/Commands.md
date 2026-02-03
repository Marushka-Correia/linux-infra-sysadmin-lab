1️) Check IP Address
ip a  - This command shows network interfaces and IP addresses.

2️) Test Network Connectivity
ping google.com - this command checks if the server can reach the internet.

- You can stop it by using the following combination of keys:
Ctrl + C

3️) Check Hostname
hostname - this command displays the server’s name.

4️) Check Listening Services and Ports
ss -tuln - this command shows services listening on network ports.
Port 22 indicates SSH.

5️) SSH Connection 
ssh sysadmin@ip_address This command is used to connect to a server remotely using SSH.

6️) Firewall Status
sudo ufw status - this command displays current firewall rules.

7️) Allow SSH Through Firewall
sudo ufw allow ssh - this command ensures SSH access is not blocked.

8️⃣ Enable Firewall
sudo ufw enable - this command activates firewall protection.


Points to remember: 
Sudo command is used in places where actions need to be done using root permissions
