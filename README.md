# Local/remote git repo
A short list of a common helpful commands  
Command line instructions

# Git global setup
git config --global user.name "username "  
git config --global user.email "xyz@gmail.com"

# To push a new project to a new repository
create an empty repository in github 
create a new repository on the command line
echo "# IOTPolicyML" >> README.md
git init
git add . 
git commit -v -m "first commit"
git remote add origin <URL to the new github repo>
git push -u origin master

# Existing Git repository
```
cd existing_repo  
git remote rename origin old-origin  
git remote add origin https://ggithub.com/alshaboti/xyz.git  
git push -u origin --all  
git push -u origin --tags  
```

# show set remote origin
Show current remote origin
```
git remote -v
```

# Redo last commit 
if you miss to add something to last commit that you still didn't push in public, then you can overrite it again as.
```
git commit -v --amend
```

# sign your commit
Assuming you have key already generated by gpg. 
You need first to configure git to use the key you want to sign with.
```
git config --global user.signingkey <keyfingerprint>
```
Then the commit you want to sign use -S option to sign it. 
```
git commit -v -S -m "this is sign commit"
```
To show the signatures
```
git log --show-signature
```
