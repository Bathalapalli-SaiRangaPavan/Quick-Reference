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
18. ```ps```: Displays information about active processes.
19. ```top```: Displays real-time information about active processes and system performance.
20. ```kill```: Terminates a process.
- ```kill -9 pid```: Force kill process id pid.
21. ```ssh```: Connects to a remote machine using Secure Shell (SSH) protocol.
22. ```scp```: Copies files securely between two machines using SSH.
23. ```tar```: Creates or extracts compressed archive files.
24. ```curl```: Sends HTTP requests and receives responses.
25. ```wget```: Downloads files from the internet.
26. ```ping```: Tests connectivity to a network host.
27. ```Sed```: Stream editor is a tool for performing search and replace operations on text files. 
28. ```awk```: For text processing that can perform a wider variety of operations. 
29. ```netstat```: Display network connections and statistics.
30. ```ifconfig```: Configure and display network interfaces.
31. ```iptables``` Configure firewall rules.
32. ```systemctl```: Control system services and display their status.
33. ```uname```: Display information about the system and its kernel.
34. ```df```: Display disk space usage.
35. ```du```: Display the size of directories and files.
36. ```mount```: Mount file systems.
37. ```umount```: Unmount file systems.
38. ```chown```: Change the owner of files and directories.
39. ```chmod```: Change the permissions of files and directories.
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
40. ```su```: Switch to a different user account.
41. ```sudo```: Execute commands with elevated privileges.
42. ```useradd```: Add a new user account.
43. ```usermod```: Modify an existing user account.
44. ```passwd```: Change a user's password.
45. ```groupadd```: Add a new group.
46. ```groupmod```: Modify an existing group.
47. ```id```: Display user and group information.
48. ```ssh-keygen```: Generate SSH keys.
49. ```ssh-copy-id```: Copy SSH keys to a remote host.
50. ```Crontab```: Allows you to schedule and automate tasks to run at specific times or intervals. 

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
