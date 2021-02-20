# Read this carefully before installing!
Boring Stuff:
Hello, I have completed this project by taking help from many sources that are available online.
I could have made this thing more complex by introducing animation to it. But it took time for me to learn the basics of it, also the deadline was knocking at the door. So I decided to go with a simple look

Now let's learn how to impliment this on Ubuntu >=16.04

## Step 1:
Go root, we don't have much time to write `sudo` as we are using virtual box.
open terminal by using Ctl+Alt+T then type `sudo su`
Enter the user password and you will be having root power!
## Step 2:
Install `plymouth-themes`
`apt install plymouth-themes`
and then install `git`
`apt install git`
## Step 3:
`cd /usr/share/plymouth/themes`
Now you are in plymouth theme directory. Now type `git clone https://github.com/EdiTechStudio/GLUG.git`
and then `cd GLUG`
now type `ls` and you should find README.md glug.script glug.png and glug.plymouth there.
## Step 4:
Now as you have verified everything, let's install this beautiful boot screen.
`update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/GLUG/glug.plymouth 1`
As we have set the priority to 1, definitely this will be the one that will be running in the boot screen. But if you do not prefer to add 1 as priority order, you can always use this command `update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/GLUG/glug.plymouth 200`or you may use any priority order number. But in this case you will be needed to write one more command and that will be:
`update-alternatives --config default.plymouth`
now look for the selection status and find the correct number for this theme. The numbers start from 0
After finding the correct number type it and press Enter.
## Final Step:
Now you have done everything, you need to keep a little bit of more patience, and you need to type this command:
`sudo update-initramfs -u`

DONE!!! You can now reboot your PC and see the magic yourself!!
