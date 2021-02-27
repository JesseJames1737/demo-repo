# Introduction

I'm having trouble figuring out how to start a repository on my local machine and push a new branch to Github

# Situation

I can create the repository and create the branch, the terminal says the push goes through fine but the new branch only contains the old information. Keeping notes so I can keep track of what I'm missing.


# Observation 1

I noticed that even though I correctly pushed, and the terminal states everything is up to date, that the text editor wanted me to save the files. I wonder if I have to save on my local machine (outside of git add .) and then push?

# Test save theory 1

I am going to make this change, save on my local machine and then git add . > git commit > git push

# Save theory seems to work!

Okay so it appears like when I make a chance, if I add > commit > push it doesn't work. Not fully. It will push the file but not the contents of the file. I'm thinking I have to save the contents of the file first so that it knows it is there. The workflow would be something like:

1. Make changes
2. Save changes on local computer (command S)
3. git add .
4. git commit -m "Comment"
5. git push (or git push -u origin master if upstream not yet set)