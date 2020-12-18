# Script For Security

For this assignment we used some monitorings tools,  two of these tools are lastb and diff. The lastb tool allows us to see failed login attempts to our system, when the -i option is used it displays the ip address. When "lasb  -i" is used in conjuctin with grep when can target "notty" which shows the failed attempt.

# For the detect_login script:
We used the lastb -i and last commands  to see failed attempts and successful logins
The output of this scrpt will be sent to a file called Suspicious_Result 
The last command which shows loginhistoy will send the results to the same Suspicous_Result file

# For Directory_File_Changes
For this script to work a copy of the /var/log directory must be created called Original_Log_Directory
The a folder in the /var/log must be created, the name could be anything you'd like.
The script will use diff to compare the copy directory with the original directory 
The output of the comparison will be sent to a file called Changes
The script will then look into the Changes file and search for any directories created using "mkdir"
