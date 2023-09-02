# Developers daily basis task with git and github

```text
 upstream : <https://github.com/MohanNalgire/InstituteManagement>

 downstream/ origin: your fork URL as example <https://github.com/krishnanalgire/InstituteManagement>

```

## steps

### step1: Pull changes from git upstream repository main branch daily when you start working

01. check remotes

    ```bash
      git remote -v
    ```

02. select upstream remote to pull code from main branch

    ```bash
      git pull upstream main
    ```

03. if conflicts resolve conflicts
 else you are good

### step2: start your work on your assigned story

2.1. create story branch

```bash
  git branch <story_branch_name> upstream/main
```

2.2. create task branches when you are working on them

```bash
    git branch <task_branch_name>
```

2.3. daily push your code to your fork task branch

  2.3.1 add your chages to staging area

  ```bash
    git add .
  ```

  2.3.2 commit your changes as per commit standards

  ```bash
        git commit -m "your commit message"
  ```

  2.3.3 check changes

  ```bash
    git status
  ```

  2.3.4 check commit logs

  ```bash
    git log --oneline
  ```

confirm your last commit message here

  2.3.5 push your changes to your branch

  ```bash
    git push origin <task_branch>
  ```

> [!IMPORTANT]
  > What to test before push your code -code level check
  >
  > - a. code is working properly
  > - b. code functionality is compeletely working on local
  > - c. add screenshots in pull request of task to story

  2.4. test your fork branch on github to verify code successfully merged or not
  on gitub

  2.5. create pull request of task to story brach and add peer reviewer to pull request
  on github
    2.5.1 got to your task branch
    2.5.2 click on contributor
    2.5.3 click on pull request
    2.5.4 select base as your story branch and from as your task branch
  
  2.6. do peer level code review in your team
    2.6.1 add your team members to reviewers from right side
    2.6.2 assignees as your name
    2.6.3 task label as per current level
    2.6.4 project if part of project
    2.6.5 add designed milestone

### step3: when story compeleted on fork then

  3.1. create story branch on upstrem repository

  3.2. create pull request from fork to upstream repository

  3.3. add reviewer for your pull request

  3.4. resolve reviewers review suggestions and push our changes once again

### step4: when story completed on story branch then

  4.1. raise pull request for release branch

  4.2. test it on multiple environment
