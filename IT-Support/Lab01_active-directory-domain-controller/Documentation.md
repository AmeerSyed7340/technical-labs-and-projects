# Installing Active Directory Domain Services and Domain Controller promotion

## Implementation
- Step 01  
  When we first log into the server we must do an initial check of a few things
  - Check the name and rename it to something appropriate for the domain
  - Check and take note of 4 important pieces of information by running *ipconfig /all* in terminal
 
- Step 02  
  We need to ensure that the server always has the same IP address. We achieve this by assigning
  - A static IP address
  - Subnet mask
  - Gateway
  - Most importantly we change the DNS to the loopback address: 127.0.0.1
    - This ensures that the server uses itself for any kind of DNS resolution

- Step 03  
  We are now ready to install Active Directory Domain Services from the Server Manager > Add roles and features > Active Directory Domain Services   
  We can follow along with the steps and install this specific role. This allows the server to be promoted to Domain Controller and enforce AD DS rules

- Step 04  
  At this stage we are prompted to promote this server to Domain Controller
  - We must choose the *Create a new domain* option and give it an appropriate name
  - We must create a *new forest*
  - We must set a password
 
- Step 05  
  The server should restart and upon a successful installation > restart we should be seeing the username prepended with the name of the domain. Example: Domain\Administration

  We are now ready to join machines to this domain.
