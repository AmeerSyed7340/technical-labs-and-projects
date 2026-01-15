# Installing Active Directory Domain Services and Domain Controller promotion

## Concept 
Active Directory (AD) is a centralized identity and directory service used to manage users, computers, and resources within a Windows domain. It enables authentication and authorization from a central location once machines and users are joined to the domain.

To implement Active Directory, a Windows Server (in this case, Windows Server 2022) is required. The server does not act as a Domain Controller by default. It must first have the Active Directory Domain Services (AD DS) role installed and then be promoted to a Domain Controller.

During promotion, a new domain is created, which also establishes a new forest. The forest represents the top-level boundary for identity and trust. Once the domain is created, users and computers can join it and be centrally managed through Active Directory.

## Check out the full step by step documented walkthrough of this lab here: [Lab 01 Documentation](Documentation.md)
