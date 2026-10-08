# Issue [1]: [Task Manager Not Opening]
encountered by [Alexander072806] on [2026-10-07]
[PC/laptop] [i am on windows 11 so not to sure if this would help with windows 10]

## Description
The issue I encountered was when attempting to open task manager it said "Task Manager has been disabled by your administrator."

## Solution:
These were the steps that I used to solve the issue.

- Press the Windows Key + R to open the Run dialog.
- Type regedit and press Enter. Click Yes if User Account Control (UAC) prompts you.
- Navigate to the following path in the left sidebar: HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Policies\System
- Look on the right-side pane for a value named DisableTaskMgr.
- Double-click DisableTaskMgr and change its Value data from 1 to 0. (Alternatively, right-click DisableTaskMgr and select Delete).
- Close the Registry Editor and restart your computer.

Try these steps listed above. They are the exact ones I followed and it allowed me to open up task manager. 
