Github Quickstart Guide

Create a repository linked to Github from the terminal

On the command line:

$ touch README.md 
# Just an empty file, need something to upload

$ git init
# Initializes the directory you are in to be connected github. The way I understand it you have two sides that are trying to connect to each other. The local directory on your computer and the github server. We want to link these two so that you can upload to that server directly from your file on your computer. To do that both files need an abstract 'flag' or 'on switch' that says 'I am ready to connect.' GIT INIT tells your computer that it is ready to connect, the first 'on switch.'

$ git add README.md
# Tells the computer that you will be adding this file to github repository. Like a staging area for all your changes. Nothing has been commited yet, but this file will be added to that staging area.

$ git commit -m "first commit" 
# Essentially says this is everything I want to commit, along with a comment describing about the uplaod. In this case it's just a simple .md file and a comment stating it's the first upload. 

$ git remote add origin http://github.com/id-Flamingo/First.git
# This is the second of the two 'on switches'. This is the repository you will be adding to. The URL can be found by going to the repository itself and clicking on the green code button which will display the HTTPS link. Going to have to come back to figure out if you can create a repository from the terminal but I'm about 90% sure you cannot.

$ git push -u origin master
# Both switches have been turned on, what files are to be commited have been staged, and now the computer uploads them to the repository.