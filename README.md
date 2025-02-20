# Pi-hole

Pi-hole is a network-wide ad blocker that acts as a DNS sinkhole, blocking ads and tracking domains for all devices on your network.

## Features
- Block ads on your entire network
- Improve your browsing speed
- Protect against online tracking
- Easy to install and use

## Prerequisites
Before setting up Pi-hole, ensure that you have the following:
- A Raspberry Pi or Linux-based device
- A working internet connection
- Access to your router’s settings (if configuring DNS)

## Installation

### **1. Update your system**
Make sure your system is up-to-date by running:


``` sudo apt update && sudo apt upgrade -y ```

### 2. Install Pi-hole
Run the following command to install Pi-hole:

bash
Copy
Edit
``` curl -sSL https://install.pi-hole.net | bash ```

### 3. Follow the on-screen prompts
The installation process will guide you through setting up Pi-hole, including selecting an upstream DNS provider and configuring your network.

<!-- Replace with your image -->
### 4. Configure your router
To ensure that all devices on your network use Pi-hole, configure your router to use the Pi-hole IP address as the DNS server.

<!-- Replace with your image -->
Usage
Once Pi-hole is installed, you can access the Pi-hole admin interface via a web browser at:

bash
Copy
Edit
``` http://<pi-hole-ip>/admin ```
Use the credentials provided during installation to log in.

<!-- Replace with your image -->
Blacklist/Whitelist Management
Blacklist: Block unwanted domains.
Whitelist: Allow specific domains that might be mistakenly blocked.
<!-- Replace with your image -->
Query Logs
You can review detailed logs of DNS queries via the admin panel.

<!-- Replace with your image -->
### Troubleshooting
If you experience any issues, refer to the following common fixes:

Ensure your router is correctly configured to use Pi-hole as the DNS server.
Check the Pi-hole logs for errors:
bash
Copy
Edit
cat /var/log/pihole.log
Restart Pi-hole if necessary:
bash
Copy
Edit
pihole restartdns

### Contribution
Feel free to contribute by forking this repository, making changes, and submitting a pull request.

python
Copy
Edit

