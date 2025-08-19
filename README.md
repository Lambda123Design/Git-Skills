# Git-Skills

Details my skills in Git

#### If we see, git status now, it will show "modified"; If we feel modification is correct, we can use "git add filename"; If need to restore previous version "git restore filename"

#### We made changes to both the files and to make sure that both are tracked we use "git add ." 

**A) Introduction, Installation and Basic Commands**

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
