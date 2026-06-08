#Git Credential Manager
-it is a secure, open source authenticator provided by git to automate and handle the authentication when you connect remotely with your repos.

-Core purpose:
    - Eliminates repetative prompts/commands.
    -Triggers modern login flows using 2FA.

- Major Services Supported:
    - Github
    - Bitbucket
    - GitLab
    - Azure repos

- Advantages:
    - Multi-Factor Auth
    - Token Management
    - Cross-platform Consistency

#Creating Github Repo:
    
    - Initialize locally:
        create a folder and move into it. 
        $git init                           ----- to initialize
        
        This creates a hidden .git folder that tracks the code history.

    - Staging:
        $ git add .                             ------ this will add all your files into staging area.
        You can also stage a single file using-
        $ git add file_name

    - Commit:
        To save your progress in local history we commit the staged files.
        Commit is very crucial to track down the erros and other problems in our project. It is used for vrsion control.

        $git commit -m  "Urs msg"

    **** Till now everything is happening in our pc, to connect to the remote repo we have to make a git repo and add it to here.

    - Connect to cloud hosting:
        $git remote add origin "URL"            ---- this is used to add origin to our project where we can access our files remotely.


#Branching and Merging:
    - Branching:
        Create a branch: git branch <name>
        Switch to a branch: git switch <name>
        Create and switch: git checkout -b <name>
        See all branches: git branch
        Delete a branch: git branch -d <name>

    Git branching allows you to isolate your work without affecting the main codebase. It creates a lightweight pointer to your commits, enabling safe experimentation and parallel development.
    
    - Merging:
        Switch to main branch: git switch main
        Merge your work: git merge <branch-name>
        Abort a messy merge: git merge --abort

         how Git combines the histories and changes from two different branches into one [Git-Branching-Basic-Branching-and-Merging].


#Cloning and pull request
    - Cloning:
        Cloning copies an existing online repository from the cloud (like GitHub) down to your local computer.

        Clone a repo: git clone <URL>
        Clone into a specific folder: git clone <URL> <folder-name>

    -Pull Requests (PR):
        A Pull Request is a web-based request to merge your branch's changes into the main codebase. It lets your team review and discuss your code before it goes live.
        
