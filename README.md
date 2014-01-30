currantest2
===========

updated by JMH on January 30, 2014 at 2:30 PM

(1) downloaded from windows.github.com
- yields GitHubSetup.exe
- may update .NET 
- installs GUI and Windows Power Shell version of git command line tool

(2) main screen (jheines) -> tools/options...
- set full name
- set email address
- set default storage directory
- can set default shell, too

(3) if a new repository that is not yet on the local system, ...
- hover over directory entry on main screen and click clone link that appears

(4) once on local system, ...
- hover and icon allows access to repository

(5) click that to get to repository page

(6) tools (gear) / open a shell here

http://stackoverflow.com/questions/1287718/how-can-i-display-my-current-git-branch-name-in-my-powershell-prompt

[{HEAD-name} +A ~B -C !D | +E ~F -G !H]

https://github.com/dahlbyk/posh-git

By default, the status summary has the following format:

[{HEAD-name} +A ~B -C !D | +E ~F -G !H !]

    {HEAD-name} is the current branch, or the SHA of a detached HEAD
        Cyan means the branch matches its remote
        Green means the branch is ahead of its remote (green light to push)
        Red means the branch is behind its remote
        Yellow means the branch is both ahead of and behind its remote
    ABCD represent the index; EFGH represent the working directory
        + = Added files
        ~ = Modified files
        - = Removed files
        ! = Conflicted files
        As in git status, index status is dark green and working directory status is dark red
        The trailing ! means there are untracked files

For example, a status of [master +0 ~2 -1 | +1 ~1 -0] corresponds to the following git status:

# On branch master
#
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#        modified:   this-changed.txt
#        modified:   this-too.txt
#        deleted:    gone.ps1
#
# Changed but not updated:
#   (use "git add <file>..." to update what will be committed)
#   (use "git checkout -- <file>..." to discard changes in working directory)
#
#        modified:   not-staged.ps1
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#        new.file
