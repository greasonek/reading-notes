# Class 3 Reading Notes

## Version Control (VCS) 
> allows to revisit various versions of a file or set of files by recording changes. Can revert to file/project, track mods and mod individuals, compare changes
- Makes easy to fix mistakes later on
- **Local VSC** = one database on hard dish to stop file changes
- **CVCS (Centralized Version Control System)** = single server storing all changes made by team of developers that can be accessed by various clients. Streamlined collaborative process, allows team members to see each others activity 
- **DVCS (Distribution Version Control)** = if CVS goes down collaborators cannot work with each other on a file or see changes/new versions. If central database corrupt and no backup, all work will be lost. DVSC prevents this by allowing clients to create mirrored repos

## Git
- *Snapshots* - Git = DVCS stores data in file system made of snapshots every commit = snapshot of file
- *Local operaions* - projects history is on local disk instead of server so can work even when not online or on VPN
- *Tracking changes* - every change tracked by git, git = gatekeeper and detects file corruption or loss
- *Loss of data* - git minimizes irreversable damage to files 
- *States* - git can reside in 3 states: 
    1. committed - securely stored in local database
    2. modified - file changed but not committed 
    3. staged - flagged file changed version to recommitted in next snapshot

## Local Repo Structure
1. Working directory: file resides here
2. Index: area for staging
3. Head: points to most recent commit

Tracked files can be modified or staged
Untracked files not in last snapshot and do not reside in staging area
- Git command: git status — determines state of file 
- Git ‘file name’ (Without quotations) tracks file 
- Git add * tracks all files in repo

### Committing file:
- Git commit -m “made changes x, y, z” commutes changed for file 
- Git commit -a commits all changes

## Pushing changes:

### Git push origin master —  
- pushes from  local branch to remote repo named origin * for cloned repos git will auto give name “origin” to the server from which you cloned 

### Stashing changes:
- Git stash — If not ready to commit changes but don’t want to lose them do