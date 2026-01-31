# Day 03 – Linux Commands Practice

## Task
Today’s goal is to **build your Linux command confidence**.

You will create a cheat sheet of commands focused on:

#### Process management
  - top/htop provides the list of process and their CPU usage
  - ps aux provides static snapshot , finding the exact pid for specific runnign process
  - "kill -9 <pid>" is forcfully killing the process that wouldn;t normally stop/shutdown
  - systemctl status <service>, its a healthcheck to see how the service is doing
  - journalctl -u <service> -f Watching the real-time error logs of a specific system service.
  
#### File system
  - "/" is a root directory
  - /bin is all bindaries are stored
  - /etc all config files are stored
  - /var/log has application and system logs
  - /home user home directory
  
  - ls -lah listing files, even hidden files in human readable format
  - df -h (disk free) to check disk space, shows how much space is left for your partitions
  - du -sh (disk usage) /var/log tell you exactly how much space is this specific folder is taking up
  - cat dumps whole file into screen
  - less allows you to scroll through the file
  - 

#### Networking troubleshooting
  - Ping <ip> used to send tiny packets to server to see server responds.
  - nslook up <domain> checks if DNS is working. it tells you if mydatab.aws.com translates to IP 
  - nc -vz <IP> <Port> (Netcat): The modern version of telnet. It’s faster and specifically designed for "scanning" to see if a connection is possible.
  - netstat -tulpn: Use this on your server to see what ports your own apps are listening on. It helps you find out if your web server actually started on port 80 or 8080.
  - curl -v to see if the API is rejecting your credentials.
