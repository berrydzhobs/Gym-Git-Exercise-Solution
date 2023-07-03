# Gym Git Exercise Solutions

This repository contains the solutions to the git exercises for the Gym Git course.


```bash
Exercise 1

#Create a project & initialize git:

$ git init
#Rename your main branch from master to main:

$ git branch -m master main
#Make changes to the project (add files, rename them, or edit them):

$ git add .
$ git commit -m "Initial commit"
#Create a GitHub repository and connect it with your project:

$ git remote add origin https://github.com/berrydzhobs/Gym-Git-Exercise-Solution.git
Push your changes to GitHub:

$ git push -u origin main
#Create a new branch dev:

$ git branch dev
#From dev, create another branch test:

$ git checkout dev
$ git branch test
#Go back to the dev branch and delete the test branch:

$ git checkout dev
$ git branch -d test


Exercise 2


Create a new home.html file, add some HTML changes, and save them:

$ touch home.html
# Add HTML changes to the file
$ git add home.html
$ git commit -m "Add home.html with HTML changes"
Stash save your current changes:

$ git stash save "Updated home.html"
Repeat the same process for a new about.html page and stash save your changes:

$ touch about.html
# Add HTML changes to the file
$ git add about.html
$ git commit -m "Add about.html with HTML changes"
$ git stash save "Updated about.html"
Repeat the same process for a new team.html page and stash save your changes:

$ touch team.html
# Add HTML changes to the file
$ git add team.html
$ git commit -m "Add team.html with HTML changes"
$ git stash save "Updated team.html"
Using stash pop, restore the changes of the about.html page:

$ git stash pop
With the help of an index, use stash pop to bring back the home.html changes:

$ git stash pop stash@{1}
Commit the current changes and push them:

$ git add .
$ git commit -m "Add home.html and about.html changes"
$ git push
Using stash pop, restore the changes of the team.html page:

$ git stash pop stash@{2}
Reset the current changes using git reset and go back to the changes without the team.html:

$ git reset HEAD
$ git checkout -- .
