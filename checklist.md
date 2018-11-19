- [] Read a line at a time, **parse the line to separate the command from its arguments**. It should then **fork and exec** the command. The parent process should **wait until the exec'd program exits** and then it should **read the next command**.
     - Note: **exit** and **cd** cannot be run through a forked child process, you will have to implement these commands on your own.
       	     - check out the **chdir()** function
- [] Read and **separate multiple commands** on one line with **;**. That is, the line ls -l ; echo hello should first run the command ls -l and then echo hello.  
    Implement **simple redirection** using **> (redirecting stdout)** and **< (redirecting stdin)**. - This will be explained in class after Thanksgiving. 
    Implement **simple pipes**, that is: ls | wc would run ls and use the output from ls as the input for wc. - This will be explained in class after Thanksgiving.
        Check out popen() for this. 