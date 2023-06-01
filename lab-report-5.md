# Lab Report 5 #

# Part 1: EdStem Post #

## Title ##

### Henri Schulz ###
Today in **Debugging**

**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

I'm using a bash terminal in VSCode on a HP Envy x360 running Windows 11 Home.

**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**

![Bash Terminal](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/7fd55836-cbae-435b-9870-1c1b5c017a7c)

The symptom I'm seeing is that the lists are not being correctly merged. I expected the result to be `[a, b, c, d, f, l, m]`, but instead got `[a, a]`, so the merge method is neither adding the same value multiple times nor creating a list of the correct length.

**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**

![Java code](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/c3ae33c1-f97a-40c2-80d2-8586560fcf03)


![Bash Script](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/b962205c-9e84-4531-b427-2ade299976c0)


![Bash Terminal](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/7fd55836-cbae-435b-9870-1c1b5c017a7c)


The failure-inducing input is `bash merge.bash "a c l m" "b d f"`.

## 1 Answer ##
#### TA Tom ###

Have you tried following along with the code you've written for these specific inputs to double-check your indices for each iteration?

##### Henri Schulz ####
Hi TA Tom,
Thank you very much for your help!

I drew it all out and discovered that I switched index1 and index2 in the first `while` loop of the `merge()` method (lines 21 and 25 specifically).

For this to work successfully, you need to be in a terminal in the `Downloads` directory, and the files `ListExamples.java` and `merge.bash` both have to be in the `Downloads` directory.

*This is the contents before fixing the bug:*
![Java code](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/c3ae33c1-f97a-40c2-80d2-8586560fcf03)

![Bash Script](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/b962205c-9e84-4531-b427-2ade299976c0)

*This is the contents after fixing the bug:*
![Fixed Java](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/ef6e036d-5607-401d-ab32-59ae2715145e)

I changed `index2` in line 21 to `index1` and `index1` in line 25 to `index2`.

![Bash Script](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/b962205c-9e84-4531-b427-2ade299976c0)

No changes were made to the bash script.

This is the result of running the fixed code:





