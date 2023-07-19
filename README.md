# bug-free-system

PowerShell Computer Status Script
This script provides a GUI that displays the status of a list of computers. It pings each computer, retrieves information about its operating system and uptime, and updates the information at specified intervals. The computer list is retrieved from a text file specified by the user.

Prerequisites
The script is written in PowerShell, so you will need a Windows environment with PowerShell installed to run it.

Usage
The script does not take any parameters. To run it, simply navigate to the directory containing the script and execute the following command in PowerShell:

Copy code
.\ScriptName.ps1
Replace ScriptName.ps1 with the actual name of the script.

Input
The script will prompt you for the path to a text file containing the names of the computers you want to monitor. The text file should have one computer name per line.

Output
The script will display a window that shows the following information for each computer:

Whether it was successfully pinged
Its IP address
Its operating system
Its service pack version
Its uptime
The date and time it last booted
Refresh Interval
The information for each computer is updated at regular intervals. You can set the refresh interval in the GUI by entering a value in the "Refresh Interval (min)" field. The default refresh interval is 10 minutes.

Debugging and Warnings
If you want to enable debug messages, you can uncomment the $debugPreference="Continue" line at the top of the script.

If you want to turn off warning messages, you can uncomment the $WarningPreference="SilentlyContinue" line at the top of the script.

Closing the Program
To close the program, click the "Close" button in the GUI.

Note
The computer list file should contain the list of computers you want to monitor, one computer name per line. For example:

Copy code
Computer1
Computer2
Computer3
Please replace "Computer1", "Computer2", etc., with the actual names of your computers.
