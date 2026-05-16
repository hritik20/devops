git init 
 --initializes an empty git repository
git status
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 4 different commits each, respectively.
  (use "git pull" if you want to integrate the remote branch with yours)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   git_commands.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen

git status 
-- this tells current status of files whether it's at staging,modified unmodified ,untracked 
files basically everything
git checkout main
 -- this is to switch to main branch,checkout command is basically used switch between branches
 git add <filename>
 -- this is to add the file at staging area where file is basically ready for commit
 git commit -m "comments"
  -- this is to finally commit the file so git can track the version of your file along with hash SHA1 value which uniqually defines each commit

  git diff <hash1>..<hash2>
  -- to check the difference between previous commit and later commit
  
  
 
 
