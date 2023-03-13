## How to initialize a git repo -->
git init .

## what is .git foler 
The .git folder is a hidden folder that is automatically created by Git when you initialize a new repository using the git init command. 

- **HEAD:** This file contains a **reference to the current branch or commit being worked on**
- **objects:** This folder contains **all the data objects in the repository, including commits, trees, and blobs.**
- **refs:** This folder contains **references to specific commits, such as branch and tag names.**
- **config:** This file contains the **configuration settings for the repository.**
- **hooks:** This folder contains **scripts that can be executed when certain events occur, such as committing changes or merging branches.**
- **index:** This file contains the **staging area, which is used to store changes before they are committed to the repository.**

## GIT config Files 

- **System-level configuration file:** This configuration file is located at **/etc/gitconfig** and contains settings that **apply to all users on the system.** You can **edit this file as a system administrator.**
- **Global configuration file:** This configuration file is located at **~/.gitconfig (or ~/.config/git/config on some systems)** and contains settings that apply to your user account across all Git repositories. You can **edit this file using the git config --global command.**
- **Local repository configuration file:** This configuration file is located in the **root directory of your Git repository, in a file called .git/config.** This file contains settings that apply only to that particular repository.

## what is origin in git repo ?

'Origin' is typically the name given to a remote git repo from which a local repo is cloned or from which it is pulling chnages regularly.  

For example, when you run the command "git clone https://github.com/username/repository.git",  
Git will **create a new local repository and set up a remote named "origin" that points to the GitHub repository at "https://github.com/username/repository.git"**  

## git add remote origine :  

**git remote add origin https://github.com/username/repository.git**  
The command sets up a local repo for a remote git repo.  
This will **add a new remote named "origin" and set the URL to the GitHub repository you specified.** 
Once the remote is added, you can use other Git commands such as "git push" and "git pull" to interact with the remote repository.

## common useful options with git clone -->

- **git clone --depth=1 <url>** --> clones only the latest commit 
- **git clone --branch dev <url>** -->  clones particular branch

## git sparce-checkout :

- git init
- git remote add origin <repository URL>
- git config core.sparseCheckout true
- git sparse-checkout set path1 path2
- git pull origin master ( if using sparce checkout for the first time )
- git sparce-checkout list 
  
## example .gitignore file 

```t
# Compiled class file
*.class

# Gradle
.gradle/

# Log file
*.log
```
