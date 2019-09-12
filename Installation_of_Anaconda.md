# Installation-of-Anaonda-on-Linux-Ubuntu
I have always loved to work with Linux(Ubuntu) because of its command line, better suited for Development, Installation of software and more Resource-friendly.
You can Download Ubuntu here

https://ubuntu.com/#download

Anaconda is the most popular python data science and machine learning platform, used for large-scale data processing, predictive analytics, and scientific computing. 
Anaconda distribution ships with more than 1,000 data packages, the conda command-line tool and with a desktop graphical user interface called Anaconda Navigator.

This tutorial will guide you through the steps of downloading and installing Anaconda Python Distribution on Ubuntu.
1. Retrieve the Latest Version of Anaconda

From a web browser, go to the Anaconda Downloads page , Find the latest version and copy the installer bash script

2. Download the Anaconda Bash Script

Logged into your Ubuntu 18.04 server as a sudo non-root user(open your terminal), move into the /tmp directory and use curl to download the link you copied from the Anaconda website:

$ cd /tmp$ curl -O https://repo.anaconda.com/archive/Anaconda3-5.2.0-Linux-x86_64.sh

3. Verify the Data Integrity of the Installer

Ensure the integrity of the installer with cryptographic hash verification through SHA-256 checksum:

$ sha256sum Anaconda3-5.2.0-Linux-x86_64.sh

You should see an output like the following

09f53738b0cd3bb96f5b1bac488e5528df9906be2480fe61df40e0e0d19e3d48  Anaconda3-5.2.0-Linux-x86_64.sh

    Make sure the hash printed from the command above matches the one available at the Anaconda with Python 3 on 64-bit Linux page for your appropriate Anaconda version.

4. Run the Anaconda Script

 $ bash Anaconda3-5.2.0-Linux-x86_64.sh

    You’ll receive the following output to review the license agreement by pressing ENTER until you reach the end.

OutputWelcome to Anaconda3 5.2.0

In order to continue the installation process, please review the license
agreement.
Please, press ENTER to continue
>>>
...
Do you approve the license terms? [yes|no]

When you get to the end of the license, type yes as long as you agree to the license to complete installation.

5. Complete Installation Process

Once you agree to the license, you will be prompted to choose the location of the installation. You can press ENTER to accept the default location, or specify a different location.

OutputAnaconda3 will now be installed into this location:
/home/tola/anaconda3

  - Press ENTER to confirm the location
  - Press CTRL-C to abort the installation
  - Or specify a different location below

[/home/tola/anaconda3] >>>

At this point, the installation will proceed. Note that the installation process takes some time.

6. Select Options

Once installation is complete, you’ll receive the following output:

Output
...
installation finished.
Do you wish the installer to prepend the Anaconda3 install location
to PATH in your /home/tola/.bashrc ? [yes|no]
[no] >>>

It is recommended that you type yes to use the conda command.

Next, you will be prompted to download Visual Studio Code, which you can learn more about from the official VSCode website.

Type yes to install and no to decline.

7. Activate Installation

You can now activate the installation with the following command:

$  source ~/.bashrc

8. Test Installation

Use the conda command to test the installation and activation:

$  conda list

To display information about current conda install type:

$  conda info

9. Updating Anaconda

first update the conda tool with:

$    conda update conda

When prompted to confirm the update, type y to proceed.

Once conda is updated, proceed with the Anaconda update:

$    conda update anaconda

Same as with the previous command, when prompted, type y to proceed.

You should regularly update your Anaconda installation.
