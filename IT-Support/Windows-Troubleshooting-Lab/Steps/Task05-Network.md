# Task 05 - Network Diagnostics

## Purpose
To verify that the system has functional network connectivity and that key network components (IP configuration, DNS, gateway, adapters) are operating normally.

## Tools Used  
  - Command Prompt (cmd)  
  - Windows Settings → Network & Internet  
  - Network Connections (ncpa.cpl)  
  - Task Manager → Performance → Ethernet/Wi-Fi  
  - Resource Monitor → Network tab (optional)  
  
## Procedure  
  - Check network adapter status  
    - Settings → Network & Internet → Status  
    - Confirm adapter is Enabled
    - Shows Connected
    - No red X or “Unidentified Network”  
  - Verify IP configuration
    - Run in Command Prompt: ipconfig /all  
    - Collect IPv4 address  
    - Default gateway  
    - DNS servers  
    - DHCP enabled  
    - Adapter details
  - Test local connectivity  
    - ping 127.0.0.1
    - ping deafault gateway from ipconfig /all  
  - Test external connectivity  
    - ping 8.8.8.8
    - ping google.com  
  - Check routing table  
    - Run: route print  
    - Check default route  
    - active interfaces  
    - metric assignments  
  - Verify DNS functionality  
    - Run: nslookup google.com   
    - Confirm DNS is reachable  
    - DNS server responds  
    - Domain resolution works  
  - Review network activity  
    - *Task Manager → Performance → Ethernet/Wi-Fi*  
    - Shows link speed  
    - Active bytes sent/received  
    - Adapter name
    - *Resource Monitor → Network tab*  
    - Processes using network  
    - Network utilization  
