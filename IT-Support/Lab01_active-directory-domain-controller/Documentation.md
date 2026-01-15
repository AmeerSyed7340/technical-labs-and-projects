# Installing Active Directory Domain Services and Domain Controller promotion

## Implementation
- Step 01
  When we first log into the server we must do an initial check of a few things.
  - Check the name and rename it to something appropriate for the domain.
  - Check and take note of 4 important pieces of information by running *ipconfig /all* in terminal.
 
- Step 02
  We need to ensure that the server always has the same IP address. We achieve this by assigning
  - A static IP address
  - Subnet mask
  - Gateway
  - Most importantly we change the DNS to the loopback address: 127.0.0.1
    - This ensures that the server uses itself for any kind of DNS resolution.
