# Lab Report 4 #
This lab report will take you through the steps needed to complete the task from the Week 7 CSE 15L lab.

Before starting, this set of instructions assumes that you have already completed steps 1-3 listed in [this task description](https://ucsd-cse15l-s23.github.io/week/week7/#timing-tasks) and you currently are in an open bash terminal in VS Code.

Note: Since steps 1-3 have already been completed, these instruction start on step 4.

## 4. Log into ieng6 ##
![Logged in](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/03b8bd33-06ae-4fe1-a2d9-b83779b6bbf4)

Keys pressed:
`ssh cs15lsp23iu@ieng6.ucsd.edu<enter>`

## 5. Clone my fork of the repository from my Github account ##
![Cloned fork](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/f379d8f2-9069-451f-8c23-71370a7909ba)

Keys pressed:
`git clo<tab>git@github.com:Irnehs/lab7.git<Enter>`

## 6. Run the tests, demonstrating that they fail ##
![Failures demonstrated](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/25149514-7309-480e-bbdb-92eaf3c99090)

Keys pressed:
```
cd lab7<enter>
javac -cp ".:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar" *.java<enter>
<up><ctrl-A><right><right><right><right><delete><up><down>
<ctrl-W>org.junit.runner.JUnitCore L<tab>T<tab><backspace><enter>`
```

## 7.Edit the code file `ListExamples.java` to fix the failing test ##
![Bugs fixed](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/ba822614-b07c-42d9-9a80-d9e2baa54181)

Keys pressed:
```
vim L<tab>.<tab><enter>
?i<enter>
e
r2
:wq
```

## 8. Run the tests, demonstrating that they now succeed ##
![Fix demonstrated](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/f8214bdd-b79d-4377-877f-0baa5113adff)

Keys pressed:
```
<up><up><up><enter>
<up><up><up><enter>
```
## 9. Commit and push the resulting change to my Github account ##
![Add, commit, push to GitHub](https://github.com/Irnehs/cse15l-lab-report/assets/24259613/cf2f8b2f-9a83-4b60-99fb-b755bb09f015)

Keys pressed:
```
git add L<tab>.j<tab><enter>
git com<tab>-m "Fixed"<enter>
git push<enter>
```

