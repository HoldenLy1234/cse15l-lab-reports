# Lab Report #1
 This is a tutorial on how to log into a course-specific account on ieng6.

## Step #1 (Installing Visual Studio Code)
Installing VS Code, you'll want to go to [this website](https://code.visualstudio.com/) and click on the download for windows, or if you have a mac you can click the arrow and download it for macOS/Linux. Follow the steps and download VS Code. From here, you should open VS Code and get a page like this.
![picture taken from week1](https://ucsd-cse15l-w22.github.io/images/vscode.png) 

## Step #2 (Remotely Connecting)
After that you'll want to remotely connect to your UCSD CSE course specific account. You'll want to check whether or not you have OpenSSH if you're running windows. You can do this by opening up powershell on your computer, and using this command (Get-WindowsCapability -Online | Where-Object Name -like 'OpenSSH*'). It should return something that looks like this 

![picture](https://i.imgur.com/FAKathb.png). 

After this, you can figure out your course specific account for CSE15L using [this link](https://sdacs.ucsd.edu/~icc/index.php). After that, you can open up your terminal in VS Code, and connect to the server using the command "ssh cs15lwi22(your ID)@ieng6@ucsd.edu."

## Step #3 (Trying some commands)

You can try commands both on the remote computer that you ssh'd to, and on your computer. cd is a command that can be used to change your directory, where your command line is currently. Here I move from my computer's desktop to a folder I had on my computer. 
![cd](https://i.imgur.com/haKk1PM.png), 

you can also try the command ls, which shows you the list of files in the directory. 
![ls](https://i.imgur.com/rUmdRyz.png)

, other commands you can try are cp, cat.

## Step #4 (Moving files with scp)

You can use the command scp to move files from your home computer into the remote computer. You can use the command this way (scp (your file, in this case WhereAmI.java was used) cs15lwi22(your ID)@ieng6.ucsd.edu:~/) It will prompt for you to login with your password, like this ![scp](https://i.imgur.com/uBJ2Mzi.png). 

Once you've added it, you can check whether or not it showed up with the command (ls) in the SSH directory.

## Step #5 (Setting up an SSH Key)
You can use an SSH key so that you don't have to enter in your login information every time, you do this by going to the terminal and using the command ssh-keygen.

![keygen](blob:https://imgur.com/efea3efc-75f3-4896-a43f-60ddd47152b4) 

This is what it should look like, this will generate a key for your computer, it will generate two keys, a public one (id_rsa.pub), and a private one (id_rsa). You want to move the public key to the ssh directory using the scp command leading to the .ssh directory in the remote computer. The command is this '''scp /Users/(your name)/.ssh/id_rsa.pub cs15lwi22(yourid)@ieng6.ucsd.edu:~/.ssh/authorized_keys.'''

## Step #6 (Optimizing remote running)
You can optimize your inputs to the terminal by putting multiple commands on a single line. This for example could be something like logging onto the remote computer and checking the home directory at the same time, or compiling and running a program in the same line. This could save keystrokes just like having a ssh key saves keystrokes so you don't have to enter things. 

![sameline](blob:https://imgur.com/4718ff1d-de73-44c4-bb4a-8055de74e198) 

This is compiling and running a program at the same time.
