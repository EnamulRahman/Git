Git reset. This moves your branch pointer backward. You’ve got 3 levels: 

•--soft keeps everything staged 

•--mixed unstages but keeps the code 

•--hard deletes everything — files and commits. Use with caution. 

Reset rewrites history. It’s powerful but dangerous on shared branches. 

Now, git revert is the safer undo. It doesn’t remove a commit — it creates a new one that reverses the changes. This is the one you use in production. Keeps the log clean and shared history intact. 

Then we’ve got git cherry-pick. This one’s surgical — it takes a single commit from another branch and applies it to your current one. Great for hotfixes or pulling in just what you need without merging the whole branch. 

You’ll use all three in different contexts. Reset for local cleanups, revert for safe public fixes, and cherry-pick for targeted precision. 
