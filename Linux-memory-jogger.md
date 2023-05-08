### some commonly used Linux commands:
1. ```ls```: Lists files and directories in the current directory.
- ```ls -l```: List items in current directory and show in long format to see perimissions, size, and modification date.
- ```ls -a```: List all items in current directory, including hidden files.
- ```ls -F```: List all items in current directory and show directories with a slash and executables with a star.
- ```ls dir```: List all items in directory dir.
2. ```cd```: Changes the current working directory.
- ```cd dir```: Change directory to dir
- ```cd ..```: Go up one directory
- ```cd /```: Go to the root directory
- ```cd ~```: Go to to your home directory
- ```cd -```: Go to the last directory you were just in
3. ```pwd```: Prints the current working directory.
4. ```mkdir```: Creates a new directory.
5. ```rm```: Deletes a file or directory.
- ```rm file```: Remove file
- ```rm -r dir```: Remove directory dir recursively
7. ```mv```: Moves a file or directory.
8. ```cp```: Copies a file or directory.
- ```cp file1 file2```: Copy file1 to file2
- ```cp -r dir1 dir2```: copy directory dir1 to dir2 recursively
9. ```ln -s file link```: create symbolic link to file
10. ```cat```: Displays the contents of a file.
11. ```less```: Displays the contents of a file one page at a time.
12. ```grep```: Searches for a pattern in a file.
13. ```ps```: Displays information about active processes.
14. ```top```: Displays real-time information about active processes and system performance.
15. ```kill```: Terminates a process.
16. ```ssh```: Connects to a remote machine using Secure Shell (SSH) protocol.
17. ```scp```: Copies files securely between two machines using SSH.
18. ```tar```: Creates or extracts compressed archive files.
19. ```curl```: Sends HTTP requests and receives responses.
20. ```wget```: Downloads files from the internet.
21. ```ping```: Tests connectivity to a network host.
22. ```Sed```: stream editor is a tool for performing search and replace operations on text files. 
23. ```awk```: for text processing that can perform a wider variety of operations. 
24. ```netstat```: Display network connections and statistics.
25. ```ifconfig```: Configure and display network interfaces.
26. ```iptables``` Configure firewall rules.
27. ```systemctl```: Control system services and display their status.
28. ```uname```: Display information about the system and its kernel.
29. ```df```: Display disk space usage.
30. ```du```: Display the size of directories and files.
31. ```mount```: Mount file systems.
32. ```umount```: Unmount file systems.
33. ```chown```: Change the owner of files and directories.
34. ```chmod```: Change the permissions of files and directories.
35. ```su```: Switch to a different user account.
36. ```sudo```: Execute commands with elevated privileges.
37. ```useradd```: Add a new user account.
38. ```usermod```: Modify an existing user account.
39. ```passwd```: Change a user's password.
40. ```groupadd```: Add a new group.
41. ```groupmod```: Modify an existing group.
42. ```id```: Display user and group information.
43. ```ssh-keygen```: Generate SSH keys.
44. ```ssh-copy-id```: Copy SSH keys to a remote host.
45. ```Crontab```: allows you to schedule and automate tasks to run at specific times or intervals. 

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
