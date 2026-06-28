# Change Username on Kali Linux

Quick way to use Kali commands to change you username on your kali linux.
#
* First open the terminal witin Kali, make note of the username that shows on top of the terminal following the word `Kali`. This is the username that you are going to be changing.
* If you are wanting to verify the your username that you are sigined into, use the `whoami` command.
*  To check the default folder that you username is under, type `pwd` to view the directory. Make sure you make note of this in order to change the username.
*  to began changing the username, type `sudo su`, and type in the password that is associated with that user account.
*  You will then be under `root` user which gives you admin rights, you may want to change the password so that you can log into the root account.
*  To change the password of the root account, type `passwd`, then enter the new password twice. Log out, and then log in as the root user.
*  Once you are logged in as the root user and change the username of a certain account, access the terminal, and then type..
    * `usermod -l [new username] -d /home/[new username] -m [old username]`
* If you get a message like "usermod: user ___ is currently used by process ___" , then you would want to take that number after the word "process" and enter in this command..
    * `kill -9 [number after process]` - This number that you are entering is the process id. 
* To then stop the process of the old username, or "kill" the process, you will then want to type this command..
    * `pkill -u [old username]`
* After this, use the same command that was used from above when you logged into the root account..
    * `usermod -l [new username] -d /home/[new username] -m [old username]`
* If you get a message like "usermod: directiry /Home/[nes username] exists", then you have successfully created the new username with a new directory.
#
Before moving forward, there are some things you may want to do to ensure that the account can be used and function as it should...
* To change the group from the old user to the new user, type this..
    * `groupmod -n [new username] [old username]` - This is simply allowing you to change features such as name and group ID. This can ensure good user management. 
* This next step is optional depending on what you prefer. To change the display name type this command.
    * `chfn -f "display name of your choice" [new username]`
* After this you can now log into the account with the new username you change it too and using the old password. 


