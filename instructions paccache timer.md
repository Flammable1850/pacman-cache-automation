The storage space on your hard drive can fill up rather quickly on an Arch system.  We can free storage space on our hard drives in several ways, one of them being to clean the pacman package manager of cached packages through a simple script, which I will show you how to create:

Step 1: 

Create a paccache.timer file: 

sudo vim /etc/systemd/system/paccache.timer

Step 2: 

To create the script, use the code from the file called paccache.timer.

Step 3: 

Aftewards, start the systemd service like so:

sudo systemctl enable paccache.timer
sudo systemctl start paccache.timer

Step 4: 

Finally, to check if the service is running use the following commands:

sudo systemctl status paccache.timer

