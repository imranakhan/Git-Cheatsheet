# Git-Cheatsheet

# To view the last 5 commits as one line items in log
git log --oneline -n 5

# To Squash multiple commits into one commit and interactively fix commit message, Very first commit becomes the main
git rebase -i HEAD~5

git push --force-with-lease   (to prevent overwriting other peoples commit with --force)

# To un-commit changes that were just commited and keep changes
git reset --soft HEAD~1

# To un-commit changes that were recently commited and discard changes (Dangerous command, will lose all changes in commit)
git reset --hard HEAD~1

# To un commit changes from last 3 commits and create one new commit
git reset --soft HEAD~3

git commit -m "New Commit"

git push --force-with-lease

# To merge down from integration branch into working branch
#Without merge commit
git pull --rebase origin develop

#with merge commit
git pull origin develop

# To update the last commits message
git commit --amend

# To update the last commits date to today
git commit --amend --date="$(date -R)"

git commit --amend --date=now
