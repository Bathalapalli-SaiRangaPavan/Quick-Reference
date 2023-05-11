### some commonly used Linux commands:
1. ```ls```: Lists files and directories in the current directory.
- ```ls -l```: List items in current directory and show in long format to see perimissions, size, and modification date.
- ```ls -a```: List all items in current directory, including hidden files.
- ```ls -F```: List all items in current directory and show directories with a slash and executables with a star.
- ```ls dir```: List all items in directory dir.
2. ```cd```: Changes the current working directory.
- ```cd dir```: Change directory to dir.
- ```cd ..```: Go up one directory.
- ```cd /```: Go to the root directory.
- ```cd ~```: Go to to your home directory.
- ```cd -```: Go to the last directory you were just in.
3. ```pwd```: Prints the current working directory.
4. ```mkdir```: Creates a new directory.
5. ```rm```: Deletes a file or directory.
- ```rm file```: Remove file.
- ```rm -r dir```: Remove directory dir recursively.
6. ```mv```: Moves a file or directory.
- ```mv file1 file2```: move (rename) file1 to file2
7. ```touch```: Create or update file.
8. ```cp```: Copies a file or directory.
- ```cp file1 file2```: Copy file1 to file2.
- ```cp -r dir1 dir2```: Copy directory dir1 to dir2 recursively.
9. ```ln -s file link```: Create symbolic link to file.
10. ```cat```: Displays the contents of a file.
11. ```less```: View file with page navigation.
12. ```head```: Output the first 10 lines of file.
13. ```tail```: Output the last 10 lines of file.
- ```tail -f file```: Output the contents of file as it grows, starting with the last 10 lines.
14. ```less```: Displays the contents of a file one page at a time.
15. ```whoami```: Who you are logged in as.
16. ```man command```: Show the manual for command.
17. ```grep```: Searches for a pattern in a file.
- ```grep pattern files```: Search for pattern in files.
- ```grep -r pattern dir```: Search recursively for pattern in dir.
- ```grep -rn pattern dir```: Search recursively for pattern in dir and show the line number found.
- ```grep -r pattern dir --include='*.ext```: Search recursively for pattern in dir and only search in files with .ext extension.
- ```command | grep pattern```: Search for pattern in the output of command.
18. ```find```: Find all instances of file in real system.
19. ```locate```: Find all instances of file using indexed database built from the updatedb command. Much faster than find.
20. ```ps```: Displays information about active processes.
21. ```top```: Displays real-time information about active processes and system performance.
22. ```kill```: Terminates a process.
- ```kill -9 pid```: Force kill process id pid.
23. ```ssh```: Connects to a remote machine using Secure Shell (SSH) protocol.
24. ```scp```: Copies files securely between two machines using SSH.
25. ```tar```: Creates or extracts compressed archive files.
- ```tar cf file.tar files```: Create a tar named file.tar containing files.
- ```tar xf file.tar```: Extract the files from file.tar.
- ```tar czf file.tar.gz files``` Create a tar with Gzip compression.
- ```tar xzf file.tar.gz```: Extract a tar using Gzip.
- ```gzip file```: Compresses file and renames it to file.gz.
- ```gzip -d file.gz```: Decompresses file.gz back to file.
26. ```curl```: Sends HTTP requests and receives responses.
27. ```wget```: Downloads files from the internet.
28. ```ping```: Tests connectivity to a network host.
29. ```Sed```: Stream editor is a tool for performing search and replace operations on text files. 
- ```sed -i 's/day/night/g' file```: Find all occurrences of day in a file and replace them with night - s means substitude and g means global - sed also supports regular expressions.
30. ```awk```: For text processing that can perform a wider variety of operations. 
31. ```netstat```: Display network connections and statistics.
32. ```ifconfig```: Configure and display network interfaces.
33. ```iptables``` Configure firewall rules.
34. ```systemctl```: Control system services and display their status.
35. ```uname```: Display information about the system and its kernel.
36. ```df```: Display disk space usage.
37. ```du```: Display the size of directories and files.
38. ```mount```: Mount file systems.
39. ```umount```: Unmount file systems.
40. ```chown```: Change the owner of files and directories.
41. ```chmod```: Change the permissions of files and directories.
- ```chmod ugo file``` - Change permissions of file to ugo - u is the user's permissions, g is the group's permissions, and o is everyone else's permissions. The values of u, g, and o can be any number between 0 and 7.
- 7 — Full permissions
- 6 — Read and Write only
- 5 — Read and Execute only
- 4 — Read only
- 3 — Write and Execute only
- 2 — Write only
- 1 — Execute only
- 0 — No permissions
- ```chmod 600 file``` — Can read and write - good for files.
- ```chmod 700 file``` — Can read, write, and execute - good for scripts.
- ```chmod 644 file``` — Can read and write, and everyone else can only read - good for web pages.
- ```chmod 755 file``` — Can read, write, and execute, and everyone else can read and execute - good for programs that you want to share.
42. ```su```: Switch to a different user account.
43. ```sudo```: Execute commands with elevated privileges.
44. ```useradd```: Add a new user account.
45. ```usermod```: Modify an existing user account.
46. ```passwd```: Change a user's password.
47. ```groupadd```: Add a new group.
48. ```groupmod```: Modify an existing group.
49. ```id```: Display user and group information.
50. ```ssh-keygen```: Generate SSH keys.
51. ```ssh-copy-id```: Copy SSH keys to a remote host.
52. ```Crontab```: Allows you to schedule and automate tasks to run at specific times or intervals. 

```
*    *    *    *    *
-    -    -    -    -
|    |    |    |    |
|    |    |    |    +----- day of the week (0 - 6) (Sunday is 0)
|    |    |    +---------- month (1 - 12)
|    |    +--------------- day of the month (1 - 31)
|    +-------------------- hour (0 - 23)
+------------------------- minute (0 - 59)
```

53. ```vi <file name>``` - vi editor is a powerful text editor 
```
#### Navigation:

h: Move the cursor left.
j: Move the cursor down.
k: Move the cursor up.
l: Move the cursor right.
0: Move to the beginning of the current line.
$: Move to the end of the current line.
gg: Move to the first line of the file.
G: Move to the last line of the file.
Ctrl+f: Move forward one page.
Ctrl+b: Move backward one page.
:n: Move to line number n.

#### Editing:

i: Insert text before the cursor.
a: Append text after the cursor.
A: Append text at the end of the current line.
o: Open a new line below the current line.
O: Open a new line above the current line.
x: Delete the character under the cursor.
dd: Delete the current line.
yy: Yank (copy) the current line.
p: Paste the previously yanked or deleted text.

#### Saving and Quitting:

:w: Save the file.
:q: Quit the editor.
:q!: Quit without saving changes.
:wq or :x: Save and quit the editor.
```

54. ```SCP```: Secure Copy is a command-line tool used to securely transfer files between a local and remote system over SSH. 
- ```scp <local_file> <remote_user>@<remote_host>:<remote_directory>```: Copy a file from local to remote.
```
scp file.txt user@example.com:/home/user/files/
```
- ```scp <remote_user>@<remote_host>:<remote_file> <local_directory>```: Copy a file from remote to local.
```
scp user@example.com:/home/user/files/file.txt /path/to/local/directory/
```
- ```scp -r <local_directory> <remote_user>@<remote_host>:<remote_directory>```: Copy a directory from local to remote.
```
scp -r my_directory user@example.com:/home/user/
```
- ```scp -r <remote_user>@<remote_host>:<remote_directory> <local_directory>``` : Copy a directory from remote to local.
```
scp -r user@example.com:/home/user/my_directory /path/to/local/directory/
```
- ```scp <local_file1> <local_file2> ... <remote_user>@<remote_host>:<remote_directory>```: Copy multiple files from local to remote.
```
scp file1.txt file2.txt user@example.com:/home/user/files/
```
- ```scp <local_directory>/<pattern> <remote_user>@<remote_host>:<remote_directory>```: Copy files matching a pattern from local to remote.
```
scp my_directory/*.txt user@example.com:/home/user/files/
```


