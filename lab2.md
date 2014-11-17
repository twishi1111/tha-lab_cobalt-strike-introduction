#### SYSTEM PROFILER

* NOTE: You MUST complete lab 1 before continuing with this lab.

1. Go to Attacks -> Web Drive-by -> System Profiler

2. Provide a Redirect URL. This is the site the system profiler will send visitors to after it collects a profile.

3. Change Local URI to something like /recon

4. Press Launch

5. Go to View -> Web Log to see who visits the system profiler

6. Go to View -> Applications to see the collected profiles

7. Now, from the THA Client Victim, go to the system profiler URL.

8. Press Refresh in the Applications tab to update the profiler information as visitors come to your system profiler.

9. Click an application and press Show Exploits.

10. Press Ctrl+A to highlight all applications, now press Show Exploits again.

11. Go to View -> Reporting -> Client Vuln. Report

12. Press Export

13. Save the vulnerability report to: `/root/THA/cobalt-strike-introduction/assets/report.pdf`

14. Open a terminal and type this command to view the PDF report:

  ```
  xpdf /root/THA/cobalt-strike-introduction/assets/report.pdf
  ```

15. Return again to your Cobalt Strike window.

16. Go to Attacks -> Web Drive By -> Manage, select your exploit and click Kill

17. You have completed this lab. You can continue to lab 3 by following the instructions found at 
    ```
    /root/THA/cobalt-strike-introduction/lab3.md
    ```
