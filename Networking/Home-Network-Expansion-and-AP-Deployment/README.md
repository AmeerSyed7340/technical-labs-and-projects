# Project Overview
This project involved replacing an existing home router, configuring a new Mercusys AC1200 router using ISP-provided network information, and repurposing an older TP-Link router as a dedicated wireless access point to expand network coverage throughout the home.

During the deployment process, the new router initially detected a PPPoE connection type. Further investigation with the Internet Service Provider revealed that the service was actually configured using static IP addressing. After obtaining the assigned network information from the ISP, the Mercusys router was successfully configured and connected to the internet.

Following the successful deployment of the primary router, the existing TP-Link router was reconfigured as a wireless access point. DHCP services were disabled on the access point to prevent conflicts with the primary router, and a static management IP address was assigned within the local network while remaining outside the DHCP address pool. The access point was connected using a LAN-to-LAN configuration and configured with a separate SSID to allow manual selection of the desired wireless network based on location within the home.

The project provided hands-on experience with router deployment, IP addressing, DHCP management, wireless networking, access point configuration, network troubleshooting, and infrastructure documentation.
