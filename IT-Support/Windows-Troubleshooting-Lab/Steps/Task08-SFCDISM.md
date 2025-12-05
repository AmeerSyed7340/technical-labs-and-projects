# Task 08 - System File & Component Repair (SFC/DISM)  

## Purpose  
To check for and repair Windows system file corruption or component store issues. Corrupted OS files can cause application crashes, login failures, slow performance, update problems, and system instability. Running SFC and DISM helps verify system integrity and restore missing or damaged files.  

## Procedure  
1. Open Command Prompt as Administrator  
   - Click Start  
   - Type cmd  
   - Right-click Command Prompt  
   - Select Run as administrator
2. Run System File Checker (SFC)
   - sfc /scannow
3. Run DISM Health Check  
   - DISM /Online /Cleanup-Image /CheckHealth  
4. Run DISM Scan (if needed)  
   - DISM /Online /Cleanup-Image /ScanHealth  
5. Run DISM Restore (if needed)  
   - DISM /Online /Cleanup-Image /RestoreHealth  
6. Re-run SFC (optional)  
   - sfc /scannow  
