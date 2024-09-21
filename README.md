# git-github
This is the first time I am using git, date: 15/9/2024.

->Create
  $git-init  --/in your folder's git bash/--

->Syncing Repositories
  $git remote add origin "link"
  $git pull origin main

->Making Changes
  $git status   --/tells about un-indexed files/--
  --/If you are making changes to a file in the folder, loca repository doesn't know about the changes. To let it know see the next step/--
  $git add edu1.txt     --/ -A for multiple files/--
  $git status

  $git commit -m "adding first commit in local repositroy"
  $git commit -a -m "adding 3 files together edu1 edu2 edu3"

  $git log

->Parallel Development
  -Branching (Branches are pointers to specific commit)
   $git branch firstbranch
   $git checkout firstbranch
   --/Now I created edu4.txt/--
   $git add edu4.txt
   $git commit -m "mking changes in firstbranch"
   $ls
   edu1 edu2 edu3 edu4 
   $git checkout main
   $ls
   edu1 edu2 edu3

  -Merging
   $git merge firstbranch
   $ls

