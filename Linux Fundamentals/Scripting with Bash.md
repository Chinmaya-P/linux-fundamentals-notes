## What I learned  
- How to create a bash script on a text editor (Mousepad)
- Syntax for a for loop within bash
- Grep, to isolate outputs from previous statements
- Cut, to isolate sections of an output based on provided delimiter
- The use of | to pipe outputs of one command into another
- Overall resulting in how to make a ping sweep script to discover machines within a given subnet.
  
## Commands and Examples  
```bash
#!/bin/bash

#IF statement to cover basic invalid input of nothing

#$1 argument to be passed in to the script by the user
if [ "$1" == "" ] 
then
echo "You forgot to enter an IP Address!"
echo "Syntax - ./pingsweep.sh 192.168.0"

else
for ip in `seq 1 254`; do 
ping -c 1 $1.$ip | grep "64 bytes" | cut -d " " -f 4 | tr -d ":" & 
done
fi
```
  
## What Confused Me  
-  At first, Bash syntax as I have previous experience (minimal) in python and C#
  
## Reflections  
-  Using Bash scripts to automate things such as ping scanning and other tedious tasks helps to improve efficiency overall.
  
  
  