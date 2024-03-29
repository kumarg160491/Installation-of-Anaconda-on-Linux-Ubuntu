
Anaconda and Jupyter Notebook Install Instructions - Ubuntu

Instructions tested with Ubuntu 18.04 64-bit and Continuum’s Anaconda 5.2.0
Install Anaconda and Jupyter Notebook

1. Open the Terminal program by going to “Show Applications” and selecting the Terminal.

2. Type the commands in red to go to the Downloads directory and download Anaconda 5.2.0. Anaconda may take a few minutes to download.
username@ubuntu:~$ cd Downloads
username@ubuntu:~/Downloads$ wget https://repo.anaconda.com/archive/Anaconda3-2019.07-Linux-x86_64.sh

3. Type the command in red to install Anaconda.
username@ubuntu:~/Downloads$ ﻿bash ./Anaconda3-2019.07-Linux-x86_64.sh

4. Press Enter to read the license agreement. Use Space to continue to the next page.
Welcome to Anaconda3 2019.07

In order to continue the installation process, please review the license agreement.
Please, press ENTER to continue

5. Type yes to accept the license terms.
Do you approve the license terms? [yes|no]
[no] >>> yes

6. Press Enter to install Anaconda to the default location.
Anaconda will now be installed into this location:
/home/username/anaconda3

- Press ENTER to confirm the location
- Press CTRL-C to abort the installation
- Or specify an different location below
[/home/username/anaconda3] >>>

7. Type yes to have Anaconda update your PATH.
installation finished.
Do you wish the installer to initialize Anaconda3
by running conda init? [yes|no]
[no] >>> yes

==> For changes to take effect, close and re-open your current shell. <==

If you'd prefer that conda's base environment not be activated on startup, set the auto_activate_base parameter to false:

conda config --set auto_activate_base false

Thank you for installing Anaconda!

8. Open a new Terminal window by going to “Show Applications” and selecting the Terminal.

9. Type the command in red to verified Anaconda was installed.
(base) username@ubuntu:~$ python --version
Python 3.7.3

10. Type the command in red to update Anaconda.
(base) username@ubuntu:~$ conda update --all --yes
Start Jupyter Notebook

1. Type the command in red to start Jupyter Notebook.
username@ubuntu:~$ jupyter notebook
