Script used for automating the process of  deleting cached versions of both unused and old versions as well as installed and uninstalled packages using the systemd.timer service.

Creating the script goes as follows:

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
