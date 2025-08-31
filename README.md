# Git-Skills

Details my skills in Git

## Basic Set of Commands to commit from Local to Github Repository - git init, git remote add origin repository_name, git add . (Adding files to Staging), git commit -m "Commit Name" (Commit the changes), git branch -M main (Setting name for Main Branch), git push -u origin main (Push to Main Branch) ; git remote set-url origin new_repository_name (To set New Repository connected to VS Code)

### git init, set the main branch, connect local to GitHub Repository, git add. (Adds all files expect files in .gitignore), git commit -m "This is my first commit", git push origin main

#### If we see, git status now, it will show "modified"; If we feel modification is correct, we can use "git add filename"; If need to restore previous version "git restore filename"

#### We made changes to both the files and to make sure that both are tracked we use "git add ." 

**A) Introduction, Installation and Basic Commands**

**B) Git Merge, Push, Checkout and Log with commands**

**C) Resolving Git Branch Merge Conflict**

**A) Introduction, Installation and Basic Commands**

1. Installed Git and opened Command Prompt, created a folder called "gittutorials", have a readme.md file, went inside that folder in command prompt, Initialized git using "git init"

#### 2. Need to initialize Basic Configurations; Search for "Git Global Config" in Google, So that it will be able to Authenticate

3. Initialize username and email id in Git using "$ git config --global user.name "Ashwath Bala S";  "$ git config --global user.email "ashwathbala0510@gmail.com"

#### Use ashwathbala510@gmail.com, when needed to commit for Lambda123Design

4. Checked for gitstatus, No commits yet and all of them were untracked files (Readme.md)

5. To track the changes: We need to add it: git add Readme.MD

#### 6. To make sure that it goes to Staging Envrionment:

git commit -m "This is the first commit"

#### Now, this will be moved to the Staging Environment; It is the place where we are keeping all the things, which needs to be pushed to the repository

If we see the git status now, it will be tracked 

7. If we see the git branch, now it will be "master" branch

8. **Renaming Master to Main Branch** - git branch -M main

9. Now if we see, git branch, it will be "main"

#### 10. To know which repository to be pushed: git remote add origin "repository name"

11. git status - It will show On main branch, commit to nothing

12. git remote -v - It shows origin,which will be the staging environment

#### 13. To push from Staging to Main: git push origin main

#### 14. Updated the Readme file saying "Subscribe to YouTube Channel"

#### 15. If we see, git status now, it will show "modified"; If we feel modification is correct, we can use "git add filename"; If need to restore previous version "git restore filename"

16. Added a new file called "test.txt"; Now if we see git status, it will show test.txt

#### 17. We made changes to both the files and to make sure that both are tracked we use "git add ." 

18. Then we can commit; git commit -m "This is my second commit

19. git push origin main

#### 20. To do cloning:

git clone "Repository Name" 

21. When we go inside and see git status there will be some new document created "New Document Created.txt" untracked files;

22. So, git status; git add .; git commit -m "This is my Third Commit"; Seeing the main branch - git branch

23. Pushing to main branch - git push origin main

**B) Git Merge, Push, Checkout and Log with commands**

1. git status - To see status of Git, no files now

2. Once we made changes and type git status, we saw txt file there

3. git add . - Adds all the files to be tracked to the staging environment

4. Once we saw git status now, we will see that file being tracked

5. **git restore --staged "FileName** -- Go to reverse

**Once we type git status now, the file will be untracked now**

6. Again did git add .

7. git reset filename - Also does the same task like git restore

**Adding again and seeing git status**

8. git diff --staged **Gives difference of what is changed but not staged**

### Real staging will happen only when the added file is committed to that staging environment

9. **Moving the added file to the staging environment:** git commit -m "This is my New Document" (Later we can move it to GitHub Repository)

10. Now running, git diff --staged --> Now nothing will be there

#### Staging Environment is like a PlayGround; Whichever needs to be committed to the Main Repository, first we will committ it over there and then push it to the GitHub Main Repository 

If we see git status now, there will be nothing because we committed to the staging environment

11. **Pushing to the Main Branch** - git push origin main

12. This is about Staging and Snapshot; Snapshot is git commit; It is basically going to take a commit snapshot, put it to Staging Part, That staging part, will be moved entirely to the GitHub Repository

#### Branching Strategy

13. git branch - Shows the main branch

14. To create a new branch in Local - git branch branch_name

This is needed because, let's say we got a new story; I will work with entire code; I will take a entire copy of main branch and cut a branch from it 

#### We will cut a Branch from the Main Branch - git branch branch_name

15. git branch - new_branch_name (It is what we created to work with)

#### 16. **Moving to the developer branch from the main branch** - git checkout developer; If we see git branch now, we will be in the new branch which we created

Whatever commit we do, it will go to the developer branch

#### 17. Now, if we see git branch, It will have all the copy of the main branch; It will also have all the copy of the files will be there 

#### 18. Now we have created a file and want to add it to developer (new_branch)

git add .; git commit -m "This is the new story I am working with" (Moving it to the Staging Environment)

#### Now entire changes will be going to the developer branch

**Now if we see git status, it will be on developer branch and nothing to commit**

**git checkout - We will be able to checkout to that specific branch**

#### Let's say, Now all my work is done, I want to merge this entire commit to the main branch in the local repository itself

**19. Checkout (Going to) main branch - git checkout main**

Now if we see git branch, it will be in Main Branch

git merge - Merge the specified branch's history into the current one

### 20. Git Merge:

**git merge new_branch (developer)** 

If we see git status now, it will show that "Your branch is ahead of origin/main by 1 commit"

#### 21. Pushing to the Main Branch

git push origin main 

#### git log - Shows all commits in the current branch history 

22. git log - It will show all the commits from the previous logs that we have done

**git log -p -3 --> Show last 3 Committs**

#### Whenever we create a new branch, we also have to make sure that we commit or push entire code from that branch to the Main Repository)

### We will also see about Pull Request, and we can merge those branches too 

**C) Resolving Git Branch Merge Conflict**

**In Main Branch, Entire Code Repository will be there**

In a project, Multiple Developers/Data Scientist working;

Dev A will try to checkout a Branch to develop his own story/module

Dev B also will try to checkout a Branch to develop his own story/module

**They do because Main Branch has the entire code repository**

**Say once Dev A completes his module he will return it to the Main Branch**

When Dev B completes his module he also has to merge it to the main branch 

####  Dev A might had lot of files, in the code and in the same file, some changes might have been done by Dev B

#### In this situation there will be a "Conflict". Dev A might made some changes to File1, where Dev B might also done some changes to same File1

#### When Dev B pushes his code, there will be a error saying that some conflict has occured

Let's say developer A is developing a Story, he will checkout from the main branch, as it will have the entire code base repository; Once they do that they will work on their own stories **He will develop the entire module and merge to the main brnach; He will develop story and merge it**

Developer B also want to work on his story too; So parallely he will also checkout from the main branch as it is the main code repository

#### Developer A also would have made some changes in the codes and files; Same changes might have happened where developer B is also working; In this scenario there will be a conflict; Because Developer A might have done some 

#### We will learn to Resolve Conflict, it is more about Resolving Conflict

**1. Created a GitHub Repository;**

**2. Created a "Git Merge Conflict" Folder in Local Windows and created "Dev A", "Dev B" folders inside it**

#### Opened Command Prompt

3. cd folder path; git clone "copy paste link from github repo"

4. Went inside "Dev A and Dev B" both folders and cloned same repo from GitHub to solve conflict issues

5. In Both Dev Folders we will do the coding and work and will try to see conflict

6. Going to Application and typing "Git Branch" **It is a Main Branch**

#### 7. Switching to developera branch using "git checkout developera"

git status - No changes there

#### 8. Going to Dev A Readme file and adding "Adding Dev A Story"

9. Now if we see git status, we will see Readme file to be tracked

10. git add. **(Krish Missed in his Video)**

11. git commit -m "Developer A Story Changes"

Seeing branch - git branch - developera

#### 12. Checkout to the Main Branch so that we can get it merged to the developer A branch

**git merge developera**

13. git status - Nothing is there; git branch - It is Main Branch

#### After Developer A completes his own Story, he has to push it to the main branch 

#### Now we just merged Developer A branch to the Main Branch; Now we will push this Main Branch to the Main Repository

#### 14. git push origin main

#### If we go and see in Github, we can see that 2 commits, Update Application and adding Developer A Story 

#### Developer B might also be working on the same branch

#### Changes has gone to the main repository over here; Before that only main copy is taken by Dev B

#### 15. Creating a new branch "git branch developerb"; git checkout developerb 

#### Making changes in Dev B Readme File; "Updated Application Dev B"

#### 16. git status; One change will be there; git add .; git commit -m "Developer B Commit"

git status, nothing will be there

#### 17. Going to the main branch; git checkout main

#### 18. Merging Developer and Main Branch; git merge developerb 

#### We have to push it to the main branch; But Developer A has already pushed some changes over there; Let's see if we are getting any error

#### 19. git push origin main -- We got Error

#### 20. git pull - We see conflict because Developer A pushed some file to the main branch over the same file 

#### We have to do changes to the file (Readme.txt) manually before pushing to Main Branch 

#### We have to do this conflict seriously, because when coding in bigger files, there might be functions or modules that may be integrated or there may be changes in previous function of the module; We need to merge that conflict in a very proper way; Otherwise it is a complete mess

#### If not, we would just overwrite others code 

#### Once merging is done;

#### 21. git status; git add ., git status; git commit -m "Developer B Story" 

#### 22. git push origin main; It will work now 

#### If we go and see GitHub Repository it will work 

#### This conflict issue will happen when working in a bigger team, because parallel stories will get implemented by many developers
