# HPC Cluster
Using HPC cluster of St. George's University of London

To be able to use the HPC Cluster you need to be given an account separately to your SGUL normal account. Please ask your line manager to arrange a new HPC account for you. 

## A. How to connect to HPC for the first time
**1. Download and Install MobaXTerm (ignore if it's already installed on your Computer):**

If you are on an SGUL PC:
+ Open the SGUL AppsAnywhere program on your Desktop
+ Click on the MobaXterm and install it

If you are on your own computer:
- Download this: https://download.mobatek.net/1212019080215819/MobaXterm_Installer_v12.1.zip
- Unzip it (Right click on the downloaded file -> Extract Here)
- Install it (Double click the extacted installer)

**2. Open MobaXTerm**

Inside MobaXTerm:
- a. Click on the Session button which is located at the upper-left corner
- b. On the menu that just popped-up click the SSH button
- c. On the Remote host text box type hpc-login.sgul.ac.uk
- d. Tick the specify username box
- e. On the Specify Username text box type your given HPC username (e.d. jsmith)
- f. Click OK
- g. On the upper Menu -> click sessions -> on the opened drop-down menu -> User sessions -> hpc-login.sgul.ac.uk (your_username)
- h. It will ask for your password. Type it and then pick yes so MobaXterm will remember your password for this connection.

**3. You are inside the HPC UNIX environment!**

Now your session has been saved under the "Sessions" tab which is located under the top left corner (The one with a star next to it).
You can click Sessions and then select hpc-login.sgul.ac.uk (your_username) from the appearing saved sessions.
MobaXTerm will remember your username and password. To change your password go to Step 2 again.

For a quick overview of UNIX commands visit this page: http://cheatsheetworld.com/programming/unix-linux-cheat-sheet/
