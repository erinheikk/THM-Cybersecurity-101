# Linux Fundamentals
Fundamentals of Linux and essential commands

### Commands
whoami - tells you who you are on the system

echo - output some specific text that is provided

ls - list what is in the current folder

cd - change directory

cat - show the contents of a file (ex. cat myfolder/myfile)

pwd - print working directory - "where am I?" within the system

find - search for files by their name. For example, find -name passwords.txt

grep - searches inside for text. For example, grep "password123" passwords.txt

--help - use this option with another command (ex. ls --help) to see a list of options we can use with the command

touch - touch	- Create file

mkdir	- make directory - Create a folder

cp - copy -	Copy a file or folder

mv - move	- Move a file or folder

rm	- remove - Remove a file or folder

file - file	- Determine the type of a file

man - manual - use with another command to read the manual (ex. man ls)

ssh - secure shell login w/name and password (ex. in CLI: ssh tryhackme@"IP ADDRESS", then enter and type in pw)

su - switch user (ex. su user2), then enter and type in pw. To drop into the new user's home directory at the same time, instead of the previous user's, use -l command with su (ex. su -l user2)

r - read

w - write

x - execute

### Operators
Special characters that combine commands together

& - Runs the command, but does not wait for it to finish before you can do anything else. The command runs in the background, and is helpful for commands that might take a while to complete, or ones that you want to keep running.

&& - Runs both commands, but waits for the first command to finish first, before the next. Like a set of dominoes.

\> - Used to redirect output. We can take the output of a command and send it to a file. This operator will overwrite anything that exists in the file.

\>> - This redirector does the same thing, but instead of overwriting, it will just add the output to the bottom of the file.

### Common Directories
/etc - This root directory is one of the most important root directories on your system. The etc folder (short for etcetera) is a commonplace location to store system files that are used by your operating system

/var - "var" being short for variable data,  is one of the main root folders found on a Linux install. This folder stores data that is frequently accessed or written by services or applications running on the system. For example, log files from running services and applications are written here (/var/log), or other data that is not necessarily associated with a specific user (i.e., databases and the like).

/root - Unlike the /home directory, the /root folder is actually the home for the "root" system user. There isn't anything more to this folder other than just understanding that this is the home directory for the "root" user

/tmp - This is a unique root directory found on a Linux install. Short for "temporary", the /tmp directory is volatile and is used to store data that is only needed to be accessed once or twice. Similar to the memory on your computer, once the computer is restarted, the contents of this folder are cleared out.

### Processes
ps - provide a list of the running processes

ps aux - to see list of processes running from other users and those that don't run from a session

### Extra
nano - launches nano. Use nano to open or create files. (ex. nano myfile) Can type text directly into file through nano

wget - download files from the web via http with a url (ex. wget https://assets.tryhackme.com/additional/linux-fundamentals/part3/myfile.txt)

start a web server using python - python3 -m http.server (remember to open a new tab to run command; specify the port in the command, (ex. wget http://10.67.129.98:8000/myfile). Once file is downloaded, use the cat command to read the file

