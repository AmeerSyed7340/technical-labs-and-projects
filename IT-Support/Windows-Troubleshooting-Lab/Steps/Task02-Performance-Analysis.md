# Task 02 - Performance Analysis using Task Manager and Resource Monitor

## Purpose
Task Manager and Resource Monitor reveal what the system is doing *right now*, allowing us to detect:  

- High CPU usage
- RAM exhaustion
- Disk bottlenecks
- Background processes causing spikes
- Startup apps slowing boot time

This task helps determine whether the issue is caused by **resource overload** before moving on to deeper troubleshooting.

---

## Tools Used
1. **Task Manager**
 - Shows real-time CPU/RAM/Disk/GPU usage
 - Shows top resource-consuming processes
 - Allows ending unresponsive apps
 - Shows startup impact  

 **Why we use this:**  
Task Manager gives an immediate snapshot of overall system performance.  
This is the fastest way to identify obvious bottlenecks.  

2. **Resource Monitor**
 - Shows deeper breakdown of CPU threads
 - Shows disk read/write activity per process
 - Shows detailed RAM usage (hard faults, committed memory)
 - Shows per-process network traffic

 **Why we use this:**  
Resource Monitor exposes hidden background processes and low-level activity that Task Manager cannot show.

---

## Procedure
1. **Task Manager**
 - Right click on Taskbar and click Task Manager
 - Go to Performance Tab -> Here we can see the performance of each of the essential components of this system
   *Image*  
2. **Processes Tab** - Identify High Resrouce Processes
 - Go to Processes Tab
 - Sort by CPU, Memory and finally Disk
 - Observe any processes using more than:
     - 30%-40% CPU
     - Large RAM usage
     - 100% Disk usage
   *image*  
 - Take Note of any suspicious activity.
3. Analyze Startup Impact
 - Go to **Startup apps**
 - Sort by "Startup impact"
 - Disable any unnecessary **High Impact** apps
 *image*  
4. Deep Dive Using Resource Monitor
 - Open Resource Monitor by pressing **Win + R** → type resmon
 - Inspect the following:
    - **CPU tab** → background processes, threads  
    - **Memory tab** → Hard faults, commit size  
    - **Disk tab** → read/write operations  
    - **Network tab** → active connections
  *image*
