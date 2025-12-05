# Task 07 - Disk Health & Storage Check

## Purpose  
To verify that the system’s storage devices have sufficient free space and are operating normally. Low disk space, disk I/O bottlenecks, or failing drives can cause slow performance, login issues, application errors, update failures, and system instability.  

# Procedure  
1. Check available disk space  
   - Open File Explorer → This PC  
   - Review the free space for each drive  
   - Confirm that the primary OS drive (usually C:) has adequate free space (ideally 15–20 GB or more)  
2. Review disk performance  
   - Open Task Manager → Performance → Disk 0 (and Disk 1 if applicable)  
   - Check disk utilization levels  
   - Confirm that the disk is not stuck at 100% usage  
   - Note the drive type (SSD/HDD) and read/write activity  
3. Identify active disk usage  
   - Open Resource Monitor → Disk tab  
   - Review which processes are performing read/write operations  
   - Look for consistently high I/O activity or unresponsive processes  
