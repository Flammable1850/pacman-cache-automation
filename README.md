# pacman-cache-automation
# Repo containing a script for the automatic removal of pacman cached packages, based on a timely schedule.

# pacman's cache can fill up space rather quickly, and I have quite often found myself without storage space, one of the ways to free up space is removing the cached packages that we no longer use. 
# The following is a guide of sorts, to help you with this process: 

# Step 1:

# Be sure to download the needed package, named "pacman-contrib" 
# We can do this with the following command sudo pacman -S pacman-contrib 

# step 2:
# Create a paccache.timer file:
# sudo vim /etc/systemd/system/paccache.timer

# Step 3:

# To create the script, use the code snippet from the file called paccache.timer. 

# Step 4:

# Aftewards, start the systemd service like so:

# sudo systemctl enable paccache.timer sudo systemctl start paccache.timer

# Step 5:

# Finally, to check if the service is running use the following commands:

# sudo systemctl status paccache.timer

# P.S. Feedback would be much appriciated.

# If there are any questions, feel free to ask them as well, I will try to get to them when I can.

