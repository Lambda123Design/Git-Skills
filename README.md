# Git-Skills

Details my skills in Git

#### If we see, git status now, it will show "modified"; If we feel modification is correct, we can use "git add filename"; If need to restore previous version "git restore filename"

#### We made changes to both the files and to make sure that both are tracked we use "git add ." 

**A) Introduction, Installation and Basic Commands**

**B) Git Merge, Push, Checkout and Log with commands**

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

