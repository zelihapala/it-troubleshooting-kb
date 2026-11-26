# High CPU usage

| | |
| --- | --- |
| **Article ID** | KB0011 |
| **Category** | Windows |
| **Applies to** | Windows 11 |
| **Audience** | End user / Helpdesk |
| **Difficulty** | Medium |
| **Time needed** | 15 minutes |
| **Tested** | tested |
| **Last updated** | 2026-11-26 |
| **Tags** | cpu, fan, overheating, task manager |

## Summary
This article helps you find the program that is using the processor heavily and decide what to do about it.

## Symptoms
- The fan is loud and the laptop is hot
- Task Manager shows CPU usage close to 100%
- The computer is slow or freezes

## Cause
A program or background process is using a lot of processor power. Common causes are a browser with many tabs, a Windows Update installing, a Windows Security scan running, a stuck program, or malware.

## Resolution
1. Press Ctrl + Shift + Esc, open the Processes page and click the CPU heading to put the highest user first. Watch for 30 seconds to see if the spike is short.
2. If it is a known program such as a browser, close extra tabs or restart the program.
3. If the process is "Antimalware Service Executable", a security scan is running. Wait until it finishes.
4. If the process is "Windows Modules Installer Worker" (TiWorker.exe), an update is installing. Let it finish and restart.
5. If the process is unknown, right-click it and select "Open file location" to see where it lives. If the name or the location looks suspicious, run a full scan: Settings > Privacy & security > Windows Security > Virus & threat protection > Scan options > Full scan.
6. Restart the computer.

## Verification
CPU usage drops below about 20% when no program is open, and the fan slows down.

## Prevention
Keep the number of open browser tabs small, install updates regularly and keep Windows Security turned on.

## Escalation
Escalate if the same process stays high after a restart, or if the security scan finds threats (inform the security team). Include the process name, a screenshot of Task Manager and the steps you tried.

## Related articles
- [Slow computer](slow-computer.md)
- [Windows Update stuck](windows-update-stuck.md)
