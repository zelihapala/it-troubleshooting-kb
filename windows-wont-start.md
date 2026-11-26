# Windows will not start

| | |
| --- | --- |
| **Article ID** | KB0014 |
| **Category** | Windows |
| **Applies to** | Windows 11 |
| **Audience** | Helpdesk |
| **Difficulty** | Hard |
| **Time needed** | 45 minutes |
| **Tested** |  tested |
| **Last updated** | 2026-11-26 |
| **Tags** | boot, startup repair, recovery, safe mode |

## Summary
This article helps when Windows does not reach the sign-in screen, for example when it shows "Automatic Repair" or restarts in a loop.

## Symptoms
- The computer restarts again and again
- The screen shows "Preparing Automatic Repair" or "Automatic Repair couldn't repair your PC"
- Windows never reaches the sign-in screen

## Cause
Common causes are a failed update, damaged system files, a faulty driver or a disk problem.

## Resolution
1. Tell the user not to reset or reinstall Windows yet, because that can delete their files.
2. If Windows does not open the recovery menu by itself, turn the computer on and hold the power button to force it off as soon as the logo appears. Repeat this two or three times. Windows then opens the recovery menu (Windows Recovery Environment).
3. Select Advanced options > Troubleshoot > Advanced options > Startup Repair. Wait for it to finish.
4. If that fails, go back to Advanced options and select Startup Settings > Restart, then press 4 or F4 to start in Safe Mode. If Windows starts in Safe Mode, uninstall the last update or driver that was installed, then restart normally.
5. If that fails, select System Restore in Advanced options and choose a restore point from before the problem started.
6. If that fails, select "Uninstall Updates" in Advanced options and remove the latest quality update.

## Verification
Windows starts normally and reaches the sign-in screen, and the user's files are present.

## Prevention
Keep restore points turned on, install updates when the computer is plugged in, and back up important files regularly.

## Escalation
Escalate if none of the steps work, or if the recovery menu does not open at all (possible disk failure). Do not reset Windows without the user's permission and a backup. Include the exact message on the screen, what happened before the problem and the steps you tried.

## Related articles
- [Blue screen (BSOD)](blue-screen.md)
- [Windows Update stuck](windows-update-stuck.md)
