# Blue screen (BSOD)

## Symptom
The computer restarts with a blue screen. An error code is shown on the screen.

## Possible causes
- A faulty or incompatible driver
- Faulty RAM
- Disk errors or damaged system files
- A recently installed program or update

## Resolution
1. Write down the error code on the blue screen (for example MEMORY_MANAGEMENT). Take a photo with a phone if possible.
2. Type "reliability" in the Start menu and open "View reliability history". Note the dates of the failures.
3. Right-click the Start button, open Terminal (Admin) and type `sfc /scannow`. This finds and repairs damaged system files.
4. If a program or driver was installed recently, uninstall it.
5. Press Windows key + R, type `mdsched.exe` and run the memory (RAM) test.

## Verification
The computer runs for 48 hours without a blue screen.

## Escalation
If the error repeats, or the error code points to hardware such as RAM or the disk, escalate to the next support level. Include the error code, the dates and the steps you tried in the handover note. Tell the user to back up their files.
