## Some useful video and file

1. an introduction to git and github by Brain Yu  youtube.com https://www.youtube.com/watch?v=MJUJ4wbFm_A
2. cs 61b : http://datastructur.es/sp17/materials/guides/using-git.html
3. pro git chinese version: https://progit.bootcss.com/
4. cs 61b: quick demo of git:https://www.youtube.com/watch?v=KoPxeLqWRTY

## the workflow of git
The files fall into two categories:
1. untracked files:
2. tracked files:
  1. unmodified files: it is the same as the one in snapshots
  2. modifies files:
  3. staged files: it is designated as part of a future commit.

commit is a snapshot of all the files that you trace in your working directory at a particular time.
users must specify what exactly composes the snapshot by staging files.

+ Unstage a file that you haven\`t yet committed.
+ amend lastest commit(changing commit message or add forgotten files)
```
git add [forgetten-file]
git commit -amend
```


## some useful command for git command line

1. **git init**   initial a reposity
2. **git add**    add new sync file; the next time committ;
every time that you change the file and want to update it , you have to use this command again to show that you want to save this version and be committed.

  note: this command is to stage the changes for commit.(that is track some information from the current file. This is gonning for commit.

  For example, if you use this command but not commit yet, and then you modify this file.  
  Then you type the command *commit*, it will still commit the older (add comand )version. )

```
  a. trace a new file and show its status
  b. stage the version
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)
        modified:   gitcommand.md
Unstage a file that you haven\`t yet committed.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
        modified:   gitcommand.md:ddd
```

PS: we can use the 'git commit -a' to skip the add step;

3. **git commit -m “message comment"** ;commit the repository; save the version;
4. **git checkout + commit ID + file**   get back to the old version  
or: **git checkout --<file>** get back to the previous file.
5. **git diff**    show the difference that haven\`t be commit  
[how to read the result of diff](http://www.ruanyifeng.com/blog/2012/08/how_to_read_diff.html)   
the result of diff is a modification of the third version of diff in unix system.
6. **git log**    show the log
7. **git show**   show last time change; if you want to see the previous version message, git show + commit ID;
8. **git status**
9. **git rm**: remove from the tracing list and remove from the workspace.   
**git rm -f**: and remove the previous file stored in the repository.  
**git rm --cached <file>**: only remove cached(stored) file in the repository.


## github operation
**git clone <url>**  :  make a copy a repository; have a copy in your pc  
**git remote add <url>**    
**git push**     this is used for github, check the version; if your version is one version ahead ,then update the version. (git push only can be used in the web-sync status)  
**git pull** retrieves changes from the github


## Merge conflicts
this is used for merge code from teammates.   
It happens when you git pull from the github and the version differs with your version. It is called a merge conflicts.  
You and your teammates push the code. The github can\`t decide which one is right. Thus you should deal with the conflicts by hand.  
You need to tell the git which version that you want to use.   
