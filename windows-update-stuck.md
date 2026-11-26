# Windows Update stuck

| | |
| --- | --- |
| **Article ID** | KB0013 |
| **Category** | Windows |
| **Applies to** | Windows 11 |
| **Audience** | Helpdesk |
| **Difficulty** | Medium |
| **Time needed** | 30 minutes |
| **Tested** | tested |
| **Last updated** | 2026-11-26 |
| **Tags** | windows update, stuck, softwaredistribution |

## Summary
This article helps when Windows Update is stuck downloading or installing, or fails with an error.

## Symptoms
- An update stays at the same percentage for hours
- Windows Update shows an error code
- The computer is stuck on "Working on updates" after a restart

## Cause
Update files may be damaged, the disk may be full, or the Windows Update service may be stuck.

## Resolution
1. Wait at least one hour. Large updates can look stuck but are still working.
2. Check that at least 10 GB of disk space is free. If not, follow the article "Disk full" (KB0012).
3. Restart the computer and check Windows Update again.
4. Open Settings > System > Troubleshoot > Other troubleshooters. Next to "Windows Update", click "Run".
5. If it is still stuck, right-click the Start button and open Terminal (Admin). Run these commands one by one. The first two stop the update services, the third renames the folder where update files are stored (Windows creates a fresh one), and the last two start the services again:
   - `net stop wuauserv`
   - `net stop bits`
   - `ren C:\Windows\SoftwareDistribution SoftwareDistribution.old`
   - `net start wuauserv`
   - `net start bits`
6. Run `sfc /scannow` and then `DISM /Online /Cleanup-Image /RestoreHealth` to repair system files.
7. Restart and check for updates again.

## Verification
Windows Update downloads and installs, and shows "You're up to date".

## Prevention
Keep enough free disk space and restart the computer regularly so updates can finish.

## Escalation
Escalate if the same error code returns after step 7. Include the error code, the steps you tried and a screenshot of Windows Update.

## Related articles
- [Disk full](disk-full.md)
- [Slow computer](slow-computer.md)
