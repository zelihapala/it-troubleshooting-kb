# Disk full

| | |
| --- | --- |
| **Article ID** | KB0012 |
| **Category** | Windows |
| **Applies to** | Windows 11 |
| **Audience** | End user / Helpdesk |
| **Difficulty** | Easy |
| **Time needed** | 15 minutes |
| **Tested** | tested |
| **Last updated** | 2026-11-26 |
| **Tags** | storage, disk space, cleanup |

## Summary
This article shows how to free up disk space safely when the disk is almost full.

## Symptoms
- A message says storage space is low
- Updates fail to install
- The computer is slow

## Cause
The disk is filled by temporary files, downloads, unused programs, large files or old update files.

## Resolution
1. Open Settings > System > Storage and look at what uses the most space.
2. Click "Temporary files". Tick "Temporary files", "Recycle Bin" and "Windows Update Cleanup" if they are listed, then click "Remove files". Do not tick "Downloads" unless the user confirms they do not need those files.
3. Turn on Storage Sense in the same page so that Windows cleans temporary files automatically.
4. Open Settings > Apps > Installed apps and uninstall programs the user no longer needs.
5. Ask the user to review the Downloads folder and delete files they do not need.
6. Type "Disk Cleanup" in the Start menu, choose the C: drive and click "Clean up system files".

## Verification
Settings > System > Storage shows at least 15% free space.

## Prevention
Keep Storage Sense on. Empty the Downloads folder regularly. Store large files on cloud storage or an external drive.

## Escalation
Escalate if a very large file or folder cannot be identified, or if the disk is too small for the user's needs and needs an upgrade. Include a screenshot of the Storage page.

## Related articles
- [Slow computer](slow-computer.md)
- [Windows Update stuck](windows-update-stuck.md)
