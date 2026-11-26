# Blue screen (BSOD)

| | |
| --- | --- |
| **Article ID** | KB0010 |
| **Category** | Windows |
| **Applies to** | Windows 11 |
| **Audience** | Helpdesk |
| **Difficulty** | Medium |
| **Time needed** | 30 minutes |
| **Tested** | tested |
| **Last updated** | 2026-11-26 |
| **Tags** | bsod, blue screen, stop code, memory, sfc |

## Summary
This article helps you collect the right information and run the first checks when a computer shows a blue screen error.

## Symptoms
- The computer restarts with a blue screen
- The screen shows an error code such as MEMORY_MANAGEMENT or CRITICAL_PROCESS_DIED

## Cause
Common causes are a faulty or incompatible driver, faulty RAM, disk errors, damaged system files, or a recently installed program or update.

## Resolution
1. Write down the error code on the blue screen. Take a photo with a phone if possible.
2. Type "reliability" in the Start menu and open "View reliability history". Note the dates of the failures.
3. Right-click the Start button, open Terminal (Admin) and run `sfc /scannow`. It finds and repairs damaged system files.
4. Run `DISM /Online /Cleanup-Image /RestoreHealth` to repair the Windows image.
5. If a program or driver was installed recently, uninstall it.
6. Press Windows key + R, type `mdsched.exe` and run the memory (RAM) test. The computer restarts to run it.

## Verification
The computer runs for 48 hours without a blue screen.

## Prevention
Install drivers from the manufacturer's website, keep Windows updated and keep the computer cool and dust-free.

## Escalation
Escalate if the error repeats, or if the code points to hardware such as RAM or the disk. Include the error code, the dates, the steps you tried and their results. Tell the user to back up their files.

## Related articles
- [Windows will not start](windows-wont-start.md)
- [Slow computer](slow-computer.md)
