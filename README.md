# paccache.timer

This is a script that I use for automatically deleting cached versions of unused and old versions of installed and uninstalled packages based on when I do my system updates. using the systemd.timer service.

Creating the script goes as follows:

Step 1: 

Create a paccache.timer file: 

sudo vim /etc/systemd/system/paccache.timer

Step 2: 

To run create thos scro[t, use the code in the file called paccache.timer.  Remember that the date in the code is based on your own personal preference. 

Step 3: 

Aftewards, start the systemd service like so:

sudo systemctl enable paccache.timer
sudo systemctl start paccache.timer

Step 4: 

Finally, to check if the service is running use the following commands:

sudo systemctl status paccache.timer
