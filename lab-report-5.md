# Lab Report 5 #

# Part 1: EdStem Post #

## No Output for System.out.println() ##

### Henri Schulz ###
Today in **Debugging**

**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

I'm using a bash terminal in VSCode on a HP Envy x360 running Windows 11 Home that is logged into my cs15l account on the remote server, which is a Mac.

**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**

I'm receiving no output, when I instead expect to see the result of all the calculator options.

**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**

![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/c6110ffe-274d-434b-8f4c-125198587aaf)

The failure-inducing input is `bash calculate.sh add 1 2 sub 5 4 mult 3 1 div 5 2 lcf 10 6 lcf 4 4 lcf 13 7`.

Here are the files I'm using:

![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/77bc07bc-8875-439f-8974-fa0d7b847205)

![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/f001f68a-600e-4996-8f9d-34498940179d)
![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/d724da63-1835-41b5-bacd-85d4e7450b21)


And here is their structure. Note, all files are stored at the same depth in the same folder:

![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/ce2866f7-d0c7-4044-8c09-1e6d4385d435)

## 1 Answer ##
#### TA Tom ###

How can you check what value being passed to Java?

##### Henri Schulz ####
Hi TA Tom,

Thank you very much for your help!

![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/b37f2dab-4fa1-4c5e-bb64-1cc7b487988c)

![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/b8961893-c883-4ee4-9659-c3490c2118b2)

I used `echo $1` and found that it was only recognizing the argument "and". I looked back at lecture notes, and saw that I need to place the string I want to pass to Java in quotations since bash uses spaces to split arguments. 

![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/40b46862-d343-48cd-82a3-228ef46fb45f)

Changed entry to command line by adding quotations:

![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/3ea3ad4e-dd45-4b8f-bc6a-eaa11a81a4f9)


# Part 2: Reflection #

In the second half of this quarter, I learned how to write bash scripts, use git, and use vim which is very helpful to me because I've been able to use all three in my lab job. Instead of using Github desktop, I can now use command line git (since earlier vim popped up and I didn't know it was vim so I had no idea how to commit or exit), which makes it easier for me to work on the multiple computers in the lab since they don't all have Github desktop installed and uploads through that takes a lot more time. I've also been able to use bash scripts on my own computer




