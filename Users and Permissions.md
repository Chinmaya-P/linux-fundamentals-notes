## What I learned  
-  How to interpret the output of ls -la (The first letter representing the object type, followed by permissions for the owner, the group and other users)
- How to modify permissions of an object using chmod ( e.g. chmod +x)
- The numbered method of chmod (where 4 = read, 2= write and 1 = execute)
- How to add a user, using adduser
- How to switch user with su 
- What the contents of etc/sudoers entails (sudo config info)
- sudo -l, finding out what commands can be used as sudo
  
## Commands and Examples  
```bash
ls -la
#Creating a script file, then changing permissions to allow execution
touch NewScript.sh
sudo chmod +x NewScript.sh

#Changing perms to allow the owner of the script to read, write, execute - followed by the group being able to read and execute, with other users not being able to do anything with the script
chmod 750 NewScript.sh

#Adding a new user and then switching into their account
adduser TestUser
su TestUser

#Finding out what the new account can use using sudo
sudo -l


```
  
## What Confused Me  
-  Originally, the number system when using chmod
- The difference in shell when moving from kali into a different user, and adapting to subtle differences.
  
## Reflections  
-  This portion is a core component for future work on any CLI, understanding how user permissions work, how this can be used to then establish access control concepts.
- The danger of tampering with important config files like /etc/sudoers and how that can cause irreparable damage to a machine.
  

  
  