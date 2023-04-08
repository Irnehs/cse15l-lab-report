## Logging into a Remote Server ##
*Before starting, ensure that you know the username and password to your course-specific account*

*If you don't know your username, look it up using your AD login with [this tool](https://sdacs.ucsd.edu/~icc/index.php).*
*If you have not used this username before, or if you forgot your password, follow [this tutorial on resetting your password](https://drive.google.com/file/d/17IDZn8Qq7Q0RkYMxdiIR0o6HJ3B5YqSW/view?usp=share_link).*
 # Installing VScode #
1. Go to the [Visual Studio Code website](https://code.visualstudio.com/) and
follow the instructions to download and install it on your computer.
2. Once you have finished the installation, you should open up a window that looks like
   this (it may have different colors or a menu bar):
      ![Image](https://ucsd-cse15l-s23.github.io/images/vscode.png)
You have successfully installed VsCode! 😄
      

# Remotely Connecting #
1. Open up VSCode and open a terminal as shown below:
[Image](https://github.com/Irnehs/cse15l-lab-report/blob/main/new_terminal.png?raw=true)
2. Make sure that the terminal type is set to ==git bash==
3. Type into the terminal:
```
$ ssh scs15lsp23XX@ieng5.ucsd.edu
```
where XX should be replaced by the unique letters in your course account's username.

4. When prompted, enter your password.
   Note: It will not show you your password as you type, dont worry!
   
5. If the password prompt reappears, you have inputted the wrong pass word and must re-enter your correct password.
   
   Otherwise, you will be greated with a prompt resembling the following:
   ![Image](https://github.com/Irnehs/cse15l-lab-report/blob/main/ssh.png?raw=true)
   
6. Congrats! You have successfully established a remote connection to the computer 😄

# Trying Out A Few Commands #
1. To view a list of all files in your working directory, enter `ls`
   A list of all files in your working directory should display similar to this image:
   *IMAGE*
   
   *Note: You may have different files within your current directory but the format should be the same*
2. Type `cd Documents` to change directory in into Documents.
3. To view a list of all files
   

