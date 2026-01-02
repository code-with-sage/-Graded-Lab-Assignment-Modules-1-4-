1. uptime<br>
    uptime command will displays how long the system has been running since the last boot, the current time, number of logged-in users etc. 

2. ps -u coder<br>
     this command will list all the process running from user coder 

3. top -u coder<br>
    this command provides a real-time, continuously updating view of processes owned by the user coder. It displays CPU usage, memory consumption, process state, and priority.

4. sleep 500 &<br>
   jobs<br>
      sleep 500 & command starts a background job that does nothing for 500 seconds, demonstrating background process handling.then  jobs command  lists all active background jobs in the current shell session, showing job IDs and their running or stopped status.

5. ps -u coder -o pid,comm,ni<br>
   reniche +3 105<br>
   ps -p 105 -o pid,comm,ni<br>
       the first command displays process ID, command name, and nice value for coder’s processes. reniche +3 105 lowers the priority of process 105. The final command confirms the updated nice value, verifying the priority change took effect.

6. free -h<br>
       free cammad displays system memory usage including total, used, free, shared, buffer, and cache memory and option -h make it in human-readable units.

7. df -h ~<br>
      this command shows disk space usage of the filesystem containing the home directory. It reports total size, used space, available space, and usage percentage in human-readable format.

8. echo $0<br>
      this command will Prints the name of the currently running shell

9. uname -a > system_report.txt<br>
     this command will  retrieves complete system information including kernel name, version, architecture, and hostname, then redirects the output into system_report.txt

10. ncdu ~ <br>
      this command was not available in the courcera  labs. 
       
