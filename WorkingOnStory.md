# Developers daily basis task with git and github

## upstream : https://github.com/MohanNalgire/InstituteManagement
## downstream/ origin: your fork URL as example https://github.com/krishnanalgire/InstituteManagement

### step1: Pull changes from git upstream repository main branch daily when you start working.
1. check remotes
	```
    git remote -v
    ```

2. select upstream remote to pull code from main branch
   ```
   git pull upstream main
   ```
	
3. if conflicts resolve conflicts
	else you are good

### step2: start your work on your assigned story
1. create story branch
	```
    git branch <story_branch_name> upstream/main
    ```
    
2. create task branches when you are working on them
	```
    git branch <task_branch_name>
    ```


3. daily push your code to your fork task branch
3.1 add your chages to staging area
```
git add .
```
3.2 commit your changes as per commit standards
```
git commit -m " your commit message"
```
3.3 check changes 
```
git status
```
3.4 check commit logs
```
git log --oneline
```
confirm your last commit message here

3.5 push your changes to your branch
```
git push origin <task_branch>
```
[!CAUTION]
What to test before push your code -code level check
- a. code is working properly
- b. code functionality is compeletely working on local
- c. add screenshots in pull request of task to story

1. test your fork branch on github to verify code successfully merged or not
		on gitub

2. create pull request of task to story brach and add peer reviewer to pull request
		on github
  5.1 got to your task branch
  5.2 click on contributor 
  5.3 click on pull request
  5.4 select base as your story branch and from as your task branch
	 

1. do peer level code review in your team
	6.1 add your team members to reviewers from right side
	6.2 assignees as your name
	6.3 task label as per current level
	6.4 project if part of project
	6.5 add designed milestone


### step3: when story compeleted on fork then 
1. create story branch on upstrem repository
2. create pull request from fork to upstream repository
3. add reviewer for your pull request
4. resolve reviewers review suggestions and push our changes once again

### step4: when story completed on story branch then 
1. raise pull request for release branch
2. test it on multiple environment
