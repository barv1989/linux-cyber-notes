## Lesson 6 — Processes & Services

Process = running program  
PID = process ID  

ps aux — show processes  
kill PID — stop process (SIGTERM)  
kill -9 PID — force stop (SIGKILL)  

Ctrl + C — stop process  
Ctrl + Z — pause process 

sleep — pause execution (used in scripts)  

Script = file with commands executed automatically  

Service = background process managed by system  

systemctl start <service> — start service  
systemctl stop <service> — stop service  
systemctl status <service> — check status  

SSH = Secure Shell, remote access to server
