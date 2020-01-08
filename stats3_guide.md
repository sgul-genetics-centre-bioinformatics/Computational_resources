# STATS3 Cluster
Using STATS3 cluster of St. George's University of London

## A. How to connect to STATS3 for the first time
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
- c. On the Remote host text box type stats3.sgul.ac.uk
- d. Tick the specify username box
- e. On the Specify Username text box type your SGUL username (e.d. jsmith)
- f. Click OK
- g. On the upper Menu -> click sessions -> on the opened drop-down menu -> User sessions -> stats3.sgul.uk (your_username)
- h. It will ask for your password. Type it and then pick yes so MobaXterm will remember your password for this connection.

**3. You are inside the stats3 UNIX environment!**

Now your session has been saved under the "Sessions" tab which is located under the top left corner (The one with a star next to it).
You can click Sessions and then select stats3.sgul.ac.uk (your_username) from the appearing saved sessions.
MobaXTerm will remember your username and password. To change your password go to Step 2 again.

For a quick overview of UNIX commands visit this page: http://cheatsheetworld.com/programming/unix-linux-cheat-sheet/

## B. Organisation of STATS3

- Everytime you connect to the stats3 you'll be landed to your STATS3 home directory.  
- For the STATS3 cluster, your home directory (~) is your **SGUL H drive**.

## C. Organisation of SGUL Genetics Centre Bioinformatics Resources

Depending on the group you are working on, you will get access to one or more of the following mounted drives or a different directory:
- **Mimir Drive**: /homedirs_APittman/sgul/shares/Mimir
- **Porthos Drive**: /homedirs-porthos/sgul/shares/incc/porthos/
- **Athos Drive**: /homedirs-yjamshid/athosnew/

You can link the drive you will be working with to your home directory.
With Mimir for example you can run:
```
cd ~
ln -s /homedirs_APittman/sgul/shares/Mimir .
```

**The Genetics_Centre_Bioinformatics Directory**  

All the above-mentioned drives (or the directory assigned to you by your line-manager) contain a directory called **Genetics_Centre_Bioinformatics**  
Inside this directory you can find:
- **resources** directory: Contains all the software and reference files we are using.
  - All software should be installed inside resources directory.  
    You can only locally install a software and then you need to point to the execution file every time you need to use it.
    e.g. ~/Mimir/Genetics_Centre_Bioinformatics_Mimir/resources/samtools-1.8/samtools view sample1.bam
  - All reference files (like genome references) should be downloaded/placed inside resources/Genome_reference_files directory.

## D. How to run commands on STATS3
STATS3 runs a simple Linux CentOS distribution without a job scheduler. That means that you can run light or heavy jobs on the terminal which use single or multiple cores and monitor them using the command ```top```

