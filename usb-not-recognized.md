# USB device not recognized

| | |
| --- | --- |
| **Article ID** | KB0015 |
| **Category** | Hardware |
| **Applies to** | Windows 11 |
| **Audience** | End user / Helpdesk |
| **Difficulty** | Medium |
| **Time needed** | 15 minutes |
| **Tested** |  tested |
| **Last updated** | 2026-11-23 |
| **Tags** | usb, flash drive, device manager, disk management |

## Summary
This article helps when a USB drive, keyboard, mouse or other USB device is not recognized by Windows.

## Symptoms
- Nothing happens when the device is plugged in
- Windows shows "USB device not recognized"
- A flash drive does not appear in File Explorer

## Cause
Common causes are a faulty port or cable, a driver problem, a drive without a drive letter, or a faulty device.

## Resolution
1. Unplug the device and plug it into a different USB port. Try a port on the back of a desktop computer.
2. Try the device on another computer. If it also fails there, the device is probably faulty.
3. Restart the computer with the device unplugged, then plug it in again.
4. Right-click the Start button and open Device Manager. Look for "Unknown USB Device" or a yellow warning symbol. Right-click it and select "Uninstall device", then unplug and replug the device.
5. For a flash drive that does not appear in File Explorer, right-click the Start button and open Disk Management. If the drive is listed without a drive letter, right-click it and select "Change Drive Letter and Paths". Do not format the drive if the user has data on it.

## Verification
The device works or the drive appears in File Explorer and its files can be opened.

## Prevention
Use "Safely remove hardware" before unplugging drives and avoid damaged cables.

## Escalation
Escalate if the device fails on another computer too (replace the device), or if the drive holds important data and shows as unallocated. Do not format it. Include the device name and what Device Manager and Disk Management show.

## Related articles
- [No sound](no-sound.md)
- [Printer not printing](printer-not-printing.md)
