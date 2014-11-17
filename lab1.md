#### STARTING COBALT STRIKE

1. Run CobaltStrike

  ```
  service postgresql start
  cd /root/THA/cobalt-strike-introduction/assets/
  ./cobaltstrike
  ```

2. A connect dialog will appear, click connect.

3. Another dialog will ask if you’d like to start Metasploit’s RPC server. Press Yes.

4. Wait for Cobalt Strike to connect to Metasploit. You will see Connection Refused multiple for up to two minutes. This is normal. If something else happens, press Cancel and then press Help to troubleshoot the issue.

5. Set the LHOST variable to ensure Cobalt Strike uses the 172.16.189.5 IP address for all listeners and services by clicking: Cobalt Strike->Listeners->Set LHOST

6. Click the “set LHOST” button and set the IP address to 172.16.189.5. Press OK to exit.

7. You have completed this lab. You can continue to lab 2 by following the instructions found at 
    ```
    /root/THA/cobalt-strike-introduction/lab2.md
    ```