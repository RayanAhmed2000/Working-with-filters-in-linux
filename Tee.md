# Usage
- Tee command is used to read from standard input (like the output of a command) and write the output to both the screen (standard output) one or multiple files simultaneously
# How is it different 
- Normally, commands in Linux send output to the screen (standard output).
- tee lets you capture that output into a file while still displaying it on the screen at the same time.
```
ls -l | tee output.txt
ls -l | tee output1.txt output2.txt
```
# Options
- options are -a or --append to append or overwrite an existing file
```
ls -l | tee --append output.txt
```
