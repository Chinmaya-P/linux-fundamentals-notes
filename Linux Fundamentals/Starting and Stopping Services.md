## What I learned  
-  How to start up a web server using Kali Linux's built in Apache2 server
- How to host a HTTP server directly from the directory I'm in within the CLI using python
- How to manage system services on system bootup such as SSH using systemctl and service commands
- Upon bootup of Apache2 server, where it stores files under var/www/html, and how to access that using a web browser e.g. 192.168.0.1/TestPage (assuming the presence of a TestPage directory under var/www/html)
## Commands and Examples  
```bash
sudo service apache2 start
sudo service apache2 stop
python3 -m http.server 80
sudo systemctl enable ssh
sudo systemctl disable ssh
```
  
## What Confused Me  
-  Nothing from this section really confused me
  
## Reflections  
-  CLI confidence growing, and ability to manage system services directly from CLI without need of GUI is a very positive growth sign so far. 
  
  
  