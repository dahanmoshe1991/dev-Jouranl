revert to last commit:  
`git reset --hard HEAD`

If all you want to do is undo the act of committing, leaving everything else intact, use:  
`git reset --soft HEAD^`

If you want to undo the act of committing and everything you'd staged, but leave the work tree (your files intact):

  `git reset HEAD^`

This will unstage all files you might have staged with git add:  
`git reset`

This will revert all local uncommitted changes (should be executed in repo root):  
`git checkout .`

You can also revert uncommitted changes only to particular file or directory:  
`git checkout [some_dir|file.txt]`

Yet another way to revert all uncommitted changes (longer to type, but works from any subdirectory):  
`git reset --hard HEAD`

This will remove all local untracked files, so only git tracked files remain:  
`git clean -fdx`  
WARNING: -x will also remove all ignored files, including ones specified by .gitignore! You may want to use -n for preview of files to be deleted.

UnAdd a file/Dir (with sub files/dir -r) from commited  

 `git rm --cached -r <path>`  
 
// delete branch locally  
`git branch -d localBranchName`   

// delete branch remotely  
`git push origin --delete remoteBranchName`   

//The -p flag means "prune". After fetching, branches which no longer exist on the remote will be deleted.  
`git fetch -p`
