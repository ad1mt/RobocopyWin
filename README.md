RobocopyWin provies an easy GUI front-end to the Robocopy command that comes with Windows.
Robocopy is a command-line file backup/copy utility that comes with Windows.
The RobocopyWin config is stored in an .ini file. If you run the program with no .ini file it will create one.
To configure alternate Robocopy options, you must edit the .ini file. RobocopyWin preserves the options in the .ini file, including those you added.
If the Robocopy command is not in the path on your PC, then you can edit the .ini file executable setting to include the full path to Robocopy.
To copy files, click the [Copy Files] button.
There is no installer; unzip, build, copy the folder to a suitable location, create a shortcut to the exe file and the log file, and copy the shortcuts to your desktop/taskbar/startmenu.
Feel free to modify this program if you wish. There is no license, it is in the public domain.
There are no guarantees with this program; you should test it before using it on important data.
Here is the contents of the recommended .ini file:
=======================
[Robocopy]
Executable=ROBOCOPY.EXE
Source=C:\
Destination=D:\
CopyOptions=/COPY:DAT /E /R:0 /XA:SHO /XD "System Volume Information" "$RECYCLE.BIN"
LogOptions=/LOG:robocopy.log /V /NP
=======================
The format of the options in the .ini file are exactly as they would be used on the command line, with one or more spaces between each option.
