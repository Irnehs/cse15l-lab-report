# Lab Report 5 #

# Part 1: EdStem Post #

## Title ##

### Henri Schulz ###
Today in **Debugging**

**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

I'm using a bash terminal in VSCode on a HP Envy x360 running Windows 11 Home that is logged into my cs15l account on the remote server, which is a Mac.

**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**

I'm receiving a NumberFormatException error.
![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/b427807b-7f67-4590-a119-e634cfce83be)


**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**


![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/bacb8003-8026-48e8-9c7c-c350ac6ad57d)

![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/9ab64441-ac31-4fd2-a4d1-e11f70741d34)


## 1 Answer ##
#### TA Tom ###

Have you tried counting through each iteration of the loop in your main method?


##### Henri Schulz ####
Hi TA Tom,
Thank you very much for your help!

I counted through my main method and realized that since I increment i by only once each iteration, I end up with the string "multiply" attempting to be converted to an int by Integer.parseInt(). To fix this, I changed my incrementation amount to 3 for each iteration.

Original code:
![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/b78829a1-0704-4373-b72f-62139235ad72)

New code:
![image](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/d9366667-a61f-4cbe-9aa6-1bbc19720cda)
I changed the increment amount in line 4 from 1 to 3.







