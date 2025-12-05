# Task06 - Updates  

## Purpose  
To verify that the system is fully updated and that Windows Update is functioning correctly. This step confirms:  
- Whether updates are downloading and installing properly  
- Whether the system is missing important security or quality updates  
- Whether any updates have failed or are pending  
- Whether Windows Update components or related services are experiencing errors  

Ensuring update functionality is important because outdated systems or failed updates can cause application issues, login failures, performance problems, security vulnerabilities, and service malfunctions.  

## Procedure  
1. Open Windows Update settings
   - Go to Settings → Windows Update
   - Confirm whether the system is up to date or if updates are pending, downloaded, installing, or failing.  
2. Review update status
   - *Screenshot*
3. View Update History  
   - Quality Updates  
   - Driver Updates  
   - Definition Updates  
   - Other Updates  
   - Feature Updates (if applicable)  
4. Verify Windows Update readiness
   - If the system shows “Up to date,” press Check for updates to confirm the service responds correctly and that the system can successfully query Microsoft’s update servers.  
5. Confirm servicing component behavior
   - Scroll down on the Windows Update page and ensure:  
     - Windows Update settings load correctly  
     - No unusual messages like “Some settings are managed by your organization” (unless expected)
6. Review Update-related logs
   - Event Viewer → Applications and Services Logs → Microsoft → Windows → WindowsUpdateClient → Operational
