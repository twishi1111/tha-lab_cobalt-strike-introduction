#### WEBSITE KEYLOGGER
These steps will show you how to clone a website and add a JavaScript keylogger to it.

1. Go to Attacks -> Web Drive-by -> Clone Site

2. Pick a site that you have a throwaway login to. This site could be http://www.gmail.com, http://mail.yahoo.com, etc.

3. Type the site you picked into the Clone URL field

4. Change the Local URI value to /clone

5. Check the Log keystrokes on  cloned site box

6. Press Clone

7. Go to View -> Web Log to watch the keystrokes come in

8. Now, from THA Client Victim, go to the URL of the cloned website and try to login. Make sure you use a throwaway account for this step. Cobalt Strike keeps track of these keystrokes in both the activity logs stored on your system and in the database it shares with the Metasploit Framework.

9. Return again to your Cobalt Strike window.

10. Go to Attacks -> Web Drive By -> Manage, select your exploit and click Kill

11. You have completed this lab. You can continue to lab 4 by following the instructions found at 
    ```
    /root/THA/cobalt-strike-introduction/lab4.md
    ```