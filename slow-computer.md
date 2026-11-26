# Slow computer

| | |
| --- | --- |
| **Article ID** | KB0001 |
| **Category** | Windows |
| **Applies to** | Windows 11 |
| **Audience** | End user / Helpdesk |
| **Difficulty** | Easy |
| **Time needed** | 15 minutes |
| **Tested** | tested |
| **Last updated** | 2026-11-26 |
| **Tags** | slow, performance, startup, task manager |

## Summary
This article helps you find out why a computer is running slowly and fix the most common causes.

## Symptoms
- The computer takes a long time to start
- Programs open slowly or freeze
- The fan runs loudly all the time

## Cause
Usually one or more of these: too many programs start automatically, the disk is almost full, a program is using a lot of CPU or memory, the computer has not been restarted for a long time, or updates are pending.

## Resolution
1. Restart the computer. A restart clears memory and closes stuck background processes.
2. Press Ctrl + Shift + Esc to open Task Manager. On the Processes page, click the CPU, Memory and Disk column headings to sort. Note which program uses the most. If it is a program you know, select it and click "End task". Do not end system processes you do not recognize.
3. In Task Manager, open "Startup apps". Right-click unnecessary programs with "High" startup impact and select "Disable".
4. Open Settings > System > Storage. If less than 15% of the disk is free, follow the article "Disk full" (KB0012).
5. Open Settings > Windows Update and install any pending updates.
6. Right-click the Start button, open Terminal (Admin) and run `sfc /scannow`. This scans for damaged system files and repairs them.

## Verification
After a restart, the computer starts in a normal time. CPU and disk usage stay low in Task Manager when no program is open.

## Prevention
Restart the computer at least once a week. Keep at least 15% of the disk free. Keep the number of startup apps small.

## Escalation
Escalate if disk usage stays at 100% after these steps, or if `sfc /scannow` reports errors it cannot fix. Include in the handover note: computer model, Windows version, a screenshot of Task Manager and the steps you tried.

## Related articles
- [High CPU usage](high-cpu-usage.md)
- [Disk full](disk-full.md)
- [Windows Update stuck](windows-update-stuck.md)

## Practical Testing Evidence

The following screenshots document practical troubleshooting on Windows 11.

- [Task Manager – Resource Usage](images/KB0001-task-manager.png)
- [CPU Performance](images/KB0001-cpu-performance.png)
- [Running Processes – CPU Usage](images/KB0001-cpu-processes.png)
- [Startup Applications](images/KB0001-startup-apps.png)
