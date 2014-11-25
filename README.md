Hacker Academy
==============
http://hackeracademy.com

### COBALT STRIKE INTRODUCTION

#### Purpose
This lab will show you how to perform client-side reconnaissance using the Cobalt Strike System Profiler feature. You will assess the client-side security of your home network and generate a report at the end of this exercise.

#### Requirements
This lab requires the following THA virtual machines
* Kali
* Vulnerable Client
* Metasploitable

#### Lab Credentials

* Kali VM: `root / toor`
* Vuln Client VM: `user / password`
* Metasploitable VM: `msfadmin / msfadmin`

#### Setup

1. Boot your THA Vulnerable Client and THA Metasploitable VMs.

2. Boot your THA Kali VM and login.

3. Clone this repo on your Kali VM by opening a terminal and issuing the following command:

    ```bash
    git clone git://github.com/madsec/tha-lab_cobalt-strike-introduction /root/THA/cobalt-strike-introduction
    ```

4. In order to install CobaltStrike you'll need to enter your email address and check for the download link - you can get a free trial here: [http://www.advancedpentest.com/trial]

5. Once you've received the email then transfer the download to your Kali VM and unzip it

  ```
  mkdir /root/THA/cobalt-strike-introduction/assets
  tar zxvf cobaltstrike-trial.tgz -C /root/THA/cobalt-strike-introduction/assets
  ```

6. Install your CobaltStrike trial

  ```
  service postgresql start
  service metasploit start
  service metasploit stop
  update-java-alternatives --jre -s java-1.7.0-openjdk-amd64
  ```

##### Note
* If the Kali VM network connection continually disconnects simply reboot the VM.

#### Start the lab
* Follow the instructions for lab 1 found on your Kali machine at 
  ```
  /root/THA/cobalt-strike-introduction/lab1.md
  ```
 
