### Processes
- A **process** is a running instance of a program
- Each process has a unique **PID (Process ID)**
- Processes can consume CPU, memory, and system resources

### Services
- A **service** is a background process managed by the system
- Services are controlled using `systemctl`
- Services can be configured to start automatically at boot

### Logs
- Logs record system events, errors, and service activity
- Logs are the primary source of truth when troubleshooting issues
- `journalctl` is used to read systemd logs

---

##   Commands 

### Process Monitoring
top - this command shows you the CPU and memory details
ps aux - this shows the list of processes
kill PID - this command is used to kill a process which is running.
kill -9 PID - this command is used to **Force** Kill a process which couldnt be killed using the normal way.

### SERVICE MANAGEMENT
systemctl status ssh -Shows whether the service is running, stopped, or failed
sudo systemctl start ssh - Starts the service right now
sudo systemctl stop ssh - Stops the running service immediately
sudo systemctl enable ssh - Configures the service to start automatically at boot
sudo systemctl disable ssh  To stop unused services from running after reboot

### LOGS & TROUBLESHOOTING
Logs tell you why something failed.
journalctl - Shows all system logs
journalctl -u ssh - Shows logs only for a specific service
journalctl -n 50 - Shows the last 50 log entries
journalctl -f - Shows logs live, in real time
tail -f /var/log/syslog -Shows live updates from the system log file


