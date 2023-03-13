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
