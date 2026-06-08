#Git Ignore and file management
    - Git ignore:
        A .gitignore file is a text file placed in your repository root directory. It tells Git which files and folders to ignore, preventing private data, dependencies, or junk files from being uploaded to the cloud.

    - File Management:
        Use Git-specific commands to move, rename, or delete files so Git can update its tracking history properly.

        Check status: git status (shows which files are modified, staged, or untracked).Rename or move: git mv <old-path> <new-path> (renames or moves a file while keeping its history).
        Delete a file: git rm <file-name> (deletes the file from both Git tracking and your computer folder).
        Discard local changes: git restore <file-name> (un-does edits and resets a file back to its last committed state).


    #Merge Conflicts:
        A merge conflict happens when Git gets confused and cannot automatically combine changes.This usually happens when:
        Two people edit the exact same line of code in the exact same file on different branches.
        One person deletes a file while another person is editing it.

        - How to fix:
            1. Find broken files:
                git status. Look for the files listed under "Both modified".

                <<<<<<< HEAD
                This is your code on your current branch.
                =======
                This is their code from the branch you are merging in.
                >>>>>>> branch-name

                -<<<<<<< HEAD : shows the start of the conflict area.
                -======= : This seperates the bbranch changes from upcoming changes.
                <<<<<<<<<: This indicates the end of the conflict area.
                