# Word not responding

| | |
| --- | --- |
| **Article ID** | KB0007 |
| **Category** | Software |
| **Applies to** | Microsoft Word on Windows 11 |
| **Audience** | End user / Helpdesk |
| **Difficulty** | Easy |
| **Time needed** | 15 minutes |
| **Tested** | tested |
| **Last updated** | 2026-11-26 |
| **Tags** | word, office, freeze, autorecover, safe mode |

## Summary
This article helps when Word freezes, and explains how to recover the document.

## Symptoms
- Clicking in Word does nothing
- The window title shows "Not Responding"

## Cause
Common causes are a very large document, an add-in (a small program added to Word) causing problems, or the computer running out of memory.

## Resolution
1. Tell the user to stay calm. The work may not be lost.
2. Wait 2-3 minutes. The program sometimes recovers on its own.
3. If it does not, press Ctrl + Shift + Esc to open Task Manager, select Word and click "End task".
4. Open Word again. A "Document Recovery" pane appears on the left. Choose the most recent version and save it.
5. If the problem repeats, hold the Ctrl key while opening Word and answer Yes to the Safe Mode question. If Word works in Safe Mode, an add-in is the cause.
6. In File > Options > Save, set the AutoRecover interval to 5 minutes.

## Verification
The document is recovered and Word works normally.

## Prevention
Save often with Ctrl + S and keep AutoRecover on. Remove add-ins the user does not need.

## Escalation
Escalate if the problem happens with every document every time, because the Office installation may need a repair. Include the Word version, whether Safe Mode works and the steps you tried.

## Related articles
- [Slow computer](slow-computer.md)
- [High CPU usage](high-cpu-usage.md)
