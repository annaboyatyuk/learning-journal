Learning journal

working on it during lab on thursday 1/11 cuz i came home yesterday and had to wash my hair and sleep :/

$ git clone ( add in the link from the github website repository when you click clone or download)
a few lines will pop up 
and then cd into the new directory and from there
git remote -v
git remote add upstream (and add that same link again)
it doesnt give any feedback so type in 
git remote -v again and itll have a couple lines that say origin and a couple that say upstream

and its connected!

then to keep it updated 
git pull upstream master



git  ADD COMMIT PUSH
starting from already having a repository on github and having cloned it on tho the local computer
on the computer add the file to the repository connected to github
cd into the directory

git add
    this stages the file for commit
        to unstage a file 'git reset HEAD (yourfile)'

git commit -m ""add a description of what changed or whatever""
    this commits changes and prepares them to be pushed
         to remove commit and modify file, 'git reset --soft HEAD~1

git push origin (your-branch)
    pushes the changes into the repository

    

