# git_commands
A short list of a common helpful commands  
Command line instructions

# Git global setup
git config --global user.name "Mohammed "  
git config --global user.email "xyz@gmail.com"

# Create a new repository
git clone https://github.com/alshaboti/xyz.git  
cd xyz  
touch README.md  
git add README.md  
git commit -m "add README"  
git push -u origin master  

# Existing folder
cd existing_folder  
git init  
git remote add origin https://github.com/alshaboti/xyz.git  
git add .  
git commit -m "Initial commit"  
git push -u origin master  

# Existing Git repository
cd existing_repo  
git remote rename origin old-origin  
git remote add origin https://ggithub.com/alshaboti/xyz.git  
git push -u origin --all  
git push -u origin --tags  
