* #Basic Git Commands

  * ### Configuration
  | Sr. No. | Command | Description |
  | ------- | ------- | ----------- |
  | 1 | git config --global user.name "Ankit Patel" | Configure username used with commit|
  | 2 | git config -- global user.email "ankitpansuriya007@gmail.com" | configure email address to be used with commits |
  | 3 | gitk | Built in git GUI|
  | 4 | git config color.ui | colorfil git output|
  | 5 | git config format.pretty oneline | show log on just one line per commit|
  | 6 | git add -i | interactive adding|
  
  * ### Repository
  | Sr. No. | Command | Description |
  | ------- | ------- | ----------- |
  | 1 | git init | create a new local repository|
  | 2 | git clone /path/to/repository | create a working copy of a local repository|
  | 3 | git clone username@host:/path/to/repository | create working copy of remote repository|
  | 4 | git remote add origin *server* | to connect local repository to remote repository to |push on server
  | 5 | git remove -v | List all currently configured remore repositories|
  | 6 | git push origin master | send changes to the master branch of your remore repository|
  | 7 | git status | List the files you've changed and those you still need to add or commit|
  | 8 | git checkout -b *branchName* | create a new branch and switch to it|
  | 9 | git checkout *branchName* | switch from one branch to another|
  | 10 | git branch | List all the branches in your repo|
  | 10 | git branch -d *branchName* | delete branch from local repository|
  | 11 | git push --all origin | push all branches to your remote repository|
  | 12 | git push origin :*branchName* or git push origin --delete *branchName* | delete a branch on your remote repository |
  | 12 | git pull | fetch and merge changes on the remote server to your working directory|
  | 13 | git merge *brnachName* | to merge different branch into active branch|
  | 14 | git diff | view all the merge conflicts|
  | 14 | git diff --base *fileName* | view the conflicts against the base file|
  | 15 | git diff *sourceBranch* *targetBranch* | Preview changes before merging|
  | 16 | git fetch origin | fetch the latest history from the remote and point your local brach at it (will keep local changes as it is) |
  | 17 | git reset --hard origin/*branchName* | discard local changes and make local brnach same as remote repository |


  * ### Files
  | Sr. No. | Command | Description |
  | ------- | ------- | ----------- |
  | 1 | git add *fileName* or git add -A or git add * | add one or multiple file to stage area|
  | 2 | git commit -m "commit message" | commit changes to head|
  | 3 | git commit -a | commit any files you have added with git add and also commit any files you have changed since then |
  | 4 | git checkout -- *fileName* | If you mess us, you can replace the changes in your working tree with the last content in head (Changes added to the index, as well as new files, will be kept) |

  * ### Tags
  | Sr. No. | Command | Description |
  | ------- | ------- | ----------- |
  | 1 | git tag 1.0.0 *commitId* | tagging to mark a significant changeset/release|
  | 2 | git push --tags origin | push all tags to remote repository|

  * ### Logs
  | Sr. No. | Command | Description |
  | ------- | ------- | ----------- |
  | 1 | git log | list of commits in active branch with unique commitIds|
  | 2 | git log --pretty=oneline | display compressed log where each commit is one line|
  | 3 | git log --author=ankit patel | display commits of certain user|
  | 4 | git log --graph --oneline --decorate --all | ASCII art tree of all the branches with details |
  | 5 | git log --name-status | display only files have changed|
