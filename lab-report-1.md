# Logging into a Remote Server #
*Before starting, ensure that you know the username and password to your course-specific account*

*If you don't know your username, look it up using your AD login with [this tool](https://sdacs.ucsd.edu/~icc/index.php).*
*If you have not used this username before, or if you forgot your password, follow [this tutorial on resetting your password](https://drive.google.com/file/d/17IDZn8Qq7Q0RkYMxdiIR0o6HJ3B5YqSW/view?usp=share_link).*
## Installing VScode ##
1. Go to the [Visual Studio Code website](https://code.visualstudio.com/) and
follow the instructions to download and install it on your computer.
2. Once you have finished the installation, you should open up a window that looks like
   this (it may have different colors or a menu bar):
      ![Image](https://ucsd-cse15l-s23.github.io/images/vscode.png)
You have successfully installed VsCode! 😄
      

## Remotely Connecting ##
1. Open up VSCode and open a terminal.
2. Make sure that the terminal type is set to `git bash`
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

## Trying Out A Few Commands ##
*An example of how steps 1-7 will appear on the terminal:*
![Image](https://github.com/Irnehs/cse15l-lab-report/blob/main/try_commands.png?raw=true)

*An example of how* ```ls -a``` *in step 8 will appear on the terminal:*
 ![ls -a](ls_a.png)
1. To view a list of all files in your working directory, enter `ls`
   A list of all files in your working directory should display similar to this image:
   *IMAGE*
   
   *Note: You may have different files within your current directory but the format should be the same*
2. To view your current working directory, enter `pwd`.
3. To change directories into perl5, enter `cd perl5`
4. To list all files in perl5 with additional information, enter `ls -lat`
5. To go back up a directory, enter `cd`
6. To copy a file from the `public` cs15lsp23 account, enter
   `cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/`
7. To view the contents of `hello.txt`, enter `cat ~/hello.txt`
8. Play around with other commands such as:
   - `ls -a` (shows all files, including hidden ones which start with ```.```)
   - `ls <directory>`
   - `cat <path>`

9. To exit the remote connection, either enter `exit` or press `CTRL-D`

   

