## Overview
Used grep and awk to filter the logs on a Linux to find sudo activity, session events, and any failed attempts.

## Tools Used
- grep
- awk
- Ubuntu 26.04 (ARM) running in UTM on macOS
- Linux terminal

## What I Did
- Accessed the Linux authentication log at /var/log/auth.log
- Used grep to filter for sudo commands, sessions, and failed login attempts
- Used awk to extract for a cleaner output
- Saved results to a file for documentation 

## Findings
- All sudo commands logged were performed by me the user jn6000
- No failed login attempts were detected because it was a new VM. 
- Session open and close events recorded for each login was normal


## What I Learned
- `grep` is used to search and filter log files by keyword, 
  allowing analysts to quickly isolate relevant events
- `awk` is used to extract specific fields from log output, 
  making raw log data cleaner and easier to read
- `auth.log` records all authentication activity on a Linux 
 including sudo commands, session events, and login attempts
- The logs did not show any failed attempts which means that there is no suspicious activity to report.
