
# Slow computer

|                  |                                          |
| ---------------- | ---------------------------------------- |
| **Article ID**   | KB0001                                   |
| **Category**     | Windows                                  |
| **Applies to**   | Windows 11                               |
| **Audience**     | End user / Helpdesk                      |
| **Difficulty**   | Easy                                     |
| **Time needed**  | 15 minutes                               |
| **Tested**       | Partially tested                         |
| **Last updated** | 2026-11-26                               |
| **Tags**         | slow, performance, startup, task manager |

## Summary

Identify and resolve common causes of slow computer performance.

## Symptoms

- The computer takes longer than usual to start.
- Applications respond slowly or freeze during normal use.
- The computer fan runs loudly for long periods.

## Cause

- Too many applications run automatically during system startup.
- Applications consume excessive CPU, memory or disk resources.
- Low disk space or pending updates affect performance.

## Resolution

1. Restart the computer to clear unnecessary background processes.
2. Press Ctrl + Shift + Esc to open Task Manager.
3. Check CPU, Memory and Disk usage under Processes.
4. Close unnecessary applications without ending unknown system processes.
5. Review and disable unnecessary applications under Startup apps.
6. Check available disk space under Settings > System > Storage.
7. Check and install any pending Windows system updates.
8. Open Terminal (Admin) and run `sfc /scannow`.

## Verification

- Check whether startup time and application performance improve.
- Monitor CPU, memory and disk usage after restarting.

## Prevention

- Restart regularly and keep Windows up to date.
- Maintain free disk space and limit startup applications.

## Escalation

- Escalate if performance issues continue after troubleshooting.
- Include system details, screenshots and completed troubleshooting steps.

## Related articles

- [High CPU usage](high-cpu-usage.md)
- [Disk full](disk-full.md)
- [Windows Update stuck](windows-update-stuck.md)

## Practical Testing Evidence

### Test Purpose

- Practise troubleshooting on a fully working Windows 11 computer.
- No known performance issues were present during testing.

### Screenshots

- [Task Manager – Resource Usage](images/KB0001-task-manager.png)
- [CPU Performance](images/KB0001-cpu-performance.png)
- [Running Processes – CPU Usage](images/KB0001-cpu-processes.png)
- [Startup Applications](images/KB0001-startup-apps.png)

### Test Findings

- CPU usage temporarily reached approximately 90%.
- Memory usage remained at approximately 54% during observation.
- Running processes and startup applications were reviewed.

### Test Outcome

- Diagnostic steps were tested without changing system settings.
- No persistent performance issues were identified during testing.
- No repair was required on the working computer.
- Remaining resolution steps were not tested.
