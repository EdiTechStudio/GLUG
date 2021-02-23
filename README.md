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
Install plymouth-themes

```
apt install plymouth-themes
```
## Step 3:
Download the zip file and unzip it.
```
unzip filename.zip
```
or for .tar.gz file
```
tar xvf filename.tar.gz
```


## Step 4:
Go to the extracted folder and run the command
```
sudo dpkg -i glug-theme_1.3_all.deb
```
## warning ⚠️⚠️: Make sure you do it from command line because this package requires you to select theme priority.
## Final Step:

Simply reboot.

DONE!!! You can now reboot your PC and see the magic yourself!!
