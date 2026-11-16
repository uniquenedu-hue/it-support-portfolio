# Project 1: Windows Troubleshooting Lab

## Project Overview
This project demonstrates my practical learning in diagnosing and troubleshooting common Windows computer problems.

## Objective
To develop practical IT Support skills by investigating common laptop issues, identifying possible causes and applying appropriate troubleshooting steps.

## Environment
- Computer: HP EliteBook
- Operating System: Windows 11
- Tools: Windows Settings, Task Manager, Device Manager and Command Prompt

## Practical Activities
The following activities will be carried out and documented:

1. Investigating slow computer performance.
2. Checking available disk space.
3. Identifying applications consuming excessive CPU or memory.
4. Checking Wi-Fi connectivity.
5. Investigating common Windows application problems.

## Troubleshooting Documentation

For each activity, I will record:

- Problem reported
- Symptoms observed
- Investigation steps
- Possible cause
- Troubleshooting actions
- Outcome
- Lessons learned

## Project Status
In progress – practical exercises and screenshots will be added as they are completed.

## Skills Being Developed
- Windows troubleshooting
- Problem-solving
- Computer maintenance
- Technical documentation
- IT Support fundamentals
## Troubleshooting Findings and Results

### Initial Problem
The laptop experienced high CPU and memory usage.

- CPU usage: 72–86% during initial observations.
- Memory usage: up to 96%.
- Installed RAM: 8 GB DDR3.

### Investigation
Task Manager showed:
- VmmemWSL: approximately 2,095 MB.
- Google Chrome: approximately 880 MB.
- Visual Studio Code: approximately 189 MB.

Linux investigation also identified Jenkins running in the background.

### Actions Taken
1. Stopped the Jenkins service because it was not currently needed.
2. Closed an unused Google Drive browser tab.
3. Ran `wsl --shutdown` in Windows PowerShell.
4. Waited approximately 45 minutes before checking resource usage again.

### Final Results

| Resource | Before WSL shutdown | After WSL shutdown |
|---|---:|---:|
| CPU | 42–50% | 15–28% |
| Memory | Up to 92% | 67% |

### Conclusion
Stopping the WSL environment significantly reduced CPU and memory usage. WSL was a major contributor to the high resource usage observed during this investigation.

### Skills Demonstrated
- Windows Task Manager monitoring
- Linux process investigation
- Basic memory troubleshooting
- Windows PowerShell commands
- Identifying unnecessary background services
- Recording troubleshooting results
