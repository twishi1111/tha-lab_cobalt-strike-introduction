#### SIGNED JAVA APPLET WEB ATTACK AND PIVOTING
These steps will show you how to set up the Java Applet attack using the Java Meterpreter Payload.

1. Go to Attacks -> Web Drive By -> Signed Applet Attack

2. Click 'win32 listener->add' and fill the out the fields with fake data and click 'save'. 

    * We're not using the Windows exploit but both must be filled out before we can launch the exploit.

3. Click “Java Listener->Add” to add a listener

4. Enter “Java Meterpreter” for the name

5. Select “java/meterpreter/reverse_tcp” from the drop down Payload menu

6. Set the port to 5555

7. Click Save

8. Click Launch

9. Now, from the THA Client Victim, make sure the Java plugin is enabled in Iceweasel and then go to this URL:

10. http://172.16.189.5/mPlayer

11. Click run when the dialogue box appears

12. Return to Colbalt Strike where you should now have a Java Meterpreter shell waiting for you.

13. Right click on the icon for our compromised host in Cobalt Strike. Navigate to Meterpreter 1 -> Explore -> Post Modules

14. Browse to the post linux modules and run them by dragging the desired module to the icon for the compromised host. Note that many of these will not work on this host. Try running the find_vmx post module. Review your loot files after running them to examine the information you were able to collect. To view the loot files click 'View -> loot"

15. Set up a pivot through this host. Right click host: Meterpreter -> Pivoting -> Setup

16. Select '172.16.189.0' and click Add Pivot button.

17. Perform Nmap scan through pivot. Hosts -> Nmap Scan -> Intense Scan

18. Enter the IP address of our Metasploit VM `172.16.189.131` and press OK

19. Wait for results and notice Green Arrow to show host is reachable through pivot.

20. Select host 172.16.189.131 and then go to: Attacks -> Find Attacks

21. Once dialog lets you know attacks were found, right click host 172.16.189.131: Attack -> samba -> usermap_script

22. Leave the defaults for the exploit module and click Launch

23. Notice the Green arrow is now bright green showing we successfully exploited this host through the pivot.

24. Run the post linux module hash dump on host 172.16.189.131.

25. Review your loot to see that you successfully downloaded the shadow file and the unshadow file for cracking in John.

26. Feel free to explore these two compromised hosts and Cobalt Strike.

27. You have completed this block of instruction.