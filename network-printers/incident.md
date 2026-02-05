## Incident Title
User unable to print to network printer

## Environment
- Windows 10
- Network printer (IP-based)
- Enterprise office setup

## Issue Description
User reported that print jobs were stuck in queue and documents were not printing to the shared network printer.

## Initial Checks
- Confirmed issue is with a network printer
- Verified user system was connected to corporate network
- Checked if issue affected multiple users (no)

## Troubleshooting Steps
1. Checked printer status on user system – printer showed offline
2. Verified printer IP connectivity using ping – successful
3. Checked printer port configuration – IP mismatch found
4. Restarted Print Spooler service
5. Updated printer port with correct IP address

## Root Cause
Printer IP address had changed, but the printer port on the user system was still mapped to the old IP.

## Resolution
Updated printer port to correct IP and restarted Print Spooler service. Printing resumed successfully.

## Prevention
Configured printer with static IP / DHCP reservation to prevent IP changes.
