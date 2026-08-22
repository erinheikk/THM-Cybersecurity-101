# Windows Fundamentals
NTFS, Control Panel, Windows desktop, etc.

### The Desktop
Graphical User Interface (GUI) welcomes you after login

Start menu, taskbar, icons/tiles on the desktop is where most applications, programs, files, and folders can be found

Notifications in taskbar managed in action center

Taskbar can be managed through enabling/disabling options that may be visible or hidden

### The Windows OS
The file system used in modern versions of Windows is the New Technology File System (NTFS). 

Before NTFS, there was  FAT16/FAT32 (File Allocation Table) and HPFS (High Performance File System). You can still see FAT systems in USB/MicroSD Devices

NTFS is known as a journaling file system. In case of a failure, the file system can automatically repair the folders/files on disk using information stored in a log file. This function is not possible with FAT.

NTFS addresses many of the limitations of the previous file systems: 
Supports files larger than 4GB, Set specific permissions on folders and files, Folder and file compression, Encryption - Encryption File System (opens in new tab) or EFS

To check permissions for a file, right click and go to Properties -> Security Tab -> Group/User Names -> Permissions

Alternate Data Streams  (ADS) is a file attribute specific to Windows NTFS. Every file has at least one data stream, and ADS allows files to contain more than one stream of data. Natively, Windows Explorer doesn't display ADS to the user. There are 3rd party executables that can be used to view this data. PowerShell also gives you the ability to view ADS for files.

The Windows folder ( C:\Windows ) is traditionally known as the folder which contains the Windows operating system. The folder doesn't have to reside in the C drive necessarily. It can reside in any other drive and technically can reside in a different folder. The system environment variable for the Windows directory is %windir%

The System32 folder holds the important files that are critical for the operating system. (You should proceed with extreme caution when interacting with this folder. Accidentally deleting any files or folders within System32 can render the Windows OS inoperational)

User accounts can be Standard or Administrator: An Administrator can make changes to the system: add users, delete users, modify groups, modify settings on the system, etc. A Standard User can only make changes to folders/files attributed to the user & can't perform system-level changes, such as install programs.

Manage users through Local User and Group Mgmt: Start Menu -> Run -> lusrmgr.msc

User Account Control (UAC) will prompt users with admin access before installing a program. This feature reduces the likelihood of malware successfully compromising your system

### Settings and Control Panel
Start Menu -> Control Panel -> Programs and Features. This will list all installed applications along with their names, publishers, and versions.

### Task Manager
The Task Manager provides information about the applications and processes currently running on the system. Other information is also available, such as how much CPU and RAM are being utilized, which falls under Performance. You can access the Task Manager by right-clicking the taskbar. 

ctrl+shift+esc or ctrl+alt+delete are keyboard shortcuts which will also open the Task Mgr

### System Settings
MSConfig - the System Configuration utility for advanced troubleshooting, and its main purpose is to help diagnose startup issues.

