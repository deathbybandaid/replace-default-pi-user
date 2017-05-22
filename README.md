# replace-default-pi-user
This will help you replace the default pi user for security measures

### We are going to change the root password.
##### If you are paranoid,,, make it something secure, use a password generator if needbe. Or simply don't be connected to a network for this step.

sudo passwd root

sudo reboot

#### Log in as root, with the password you just created

wget https://raw.githubusercontent.com/deathbybandaid/replace-default-pi-user/master/replacepi.sh

bash /etc/piadvanced/renamedefaultpiuser.sh

###### This will remove the root password we added earlier and lock the account.
passwd -dl root

sudo reboot

#### after it reboots, login as your new user.
