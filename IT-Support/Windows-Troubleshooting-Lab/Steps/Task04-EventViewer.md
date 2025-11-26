# Event Viewer

## Purpose  
We check to validate assumptions from earlier tasks and pinpoint the exact cause of user-reported issues.  

## Tools Used  
1. Application Logs  
   - Application crashes  
   - Faulty programs  
   - .NET errors  
   - Third-party software issues  

2. System Logs  
   - Service failures  
   - Driver problems  
   - Windows Update errors  
   - Hardware/Disk issues  
   - Unexpected shutdowns  

3. Security Logs (Optional)  
   - Login attempts  
   - Logon failures  
   - Account lockouts  

4. Windows Logs → Setup  
   - Windows Update installation logs

5. Applications and Services Logs  
   - Specific logs from Microsoft or hardware vendors  

## Procedure  
1. Open Event Viewer  
   - Press Win + R  
   - Type eventvwr.msc  
   - Press Enter  
2. Navigate to key log areas    
   - Windows Logs → System
   - Windows Logs → Application
   - Windows Logs → Setup  
3. Filter or sort by Level  
   - Click Level to group logs:  
     - Critical
     - Error
     - Warning
     
