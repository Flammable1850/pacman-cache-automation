# pacman-cache-automation
# Repo containing scripts for the automatic removal of pacman cached packages, based on a timely schedule.

# The storage space on your hard drive can fill up rather quickly on an Arch system.  There are several ways to free up space, I will show you how to automate one of them to remove cached paccman packages by removing unused packages automatically, one a timed basis.

# Step 1:

# Create a paccache.timer file:

# sudo vim /etc/systemd/system/paccache.timer

# Step 2:

# To create the script, use the code snippet from the file called paccache.timer. 

# Step 3:

# Aftewards, start the systemd service like so:

# sudo systemctl enable paccache.timer sudo systemctl start paccache.timer

# Step 4:

# Finally, to check if the service is running use the following commands:

# sudo systemctl status paccache.timer

# P.S. Feedback would be much appriciated.

# If there are any questions, feel free to ask them as well, I will try to get to them when I can.

