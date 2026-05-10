# GitHubAssignment
assignment testing
1.
git init
touch app.py
git  status
git add .
git commit -m "first commit"   
git remote a
git remote add origin https://github.com/srikanth331gugulothu-png/GitHubAssignment 
git remote - v
git push -u origin main
2.
git status
git diff
git add .
git commit - m "feature 1 is added"

# after more changes
git add .
git commit -m "feature 2 is added"

git log
git log --oneline
3.
git checkout -b feature-update

# modify app.py

git add .
git commit - m "branch feature started"

git checkout main
git merge feature-update

git log --oneline

git branch -d feature-update

# force delete example
git checkout -b dummy-branch
git add app.py
git commit -m "Dummy commit"

git checkout main
git branch -D dummy-branch
4.
# modify files
git stash -u

git stash list
git stash apply

git add .
git commit -m "Added function"

# bad commit
git add app.py
git commit -m "added incorrect  logic"

# undo commit
git reset --soft HEAD~1

# fix and recommit
git add app.py
git commit -m "Fixed added function"

# another commit
git add app.py
git commit -m "Added subtract function"

# revert commit
git revert HEAD

# verify history
git log
git log --oneline
