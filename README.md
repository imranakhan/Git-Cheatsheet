# Git-Cheatsheet


# To Squash multiple commits into one commit and interactively fix commit message, Very first commit becomes the main
git rebase -i HEAD~5

git push --force-with-lease   (to prevent overwriting other peoples commit with --force)

# To un commit changes from last 3 commits and create one new commit
git reset --soft HEAD~3

git commit -m "New Commit"

git push --force-with-lease


