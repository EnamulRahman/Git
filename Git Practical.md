Private key and public key – can share public key  

 

Pbcopy – copies to clipboard 

 

// cat ~/.ssh/enamul.demo.pub 

 

/ git init 

 

/ git status 

 

/ git add 

 

/ git commit –m "init commit" 

 


/ git push –u origin main  

 

 

Steps: 

 

Step 1. Make sure your SSH key is added to the agent 

eval "$(ssh-agent -s)" 
ssh-add ~/.ssh/enamul.demo 
 

 

Step 2. Add your SSH public key to GitHub 

Run: 

cat ~/.ssh/enamul.demo.pub 
 

Copy the output (your public key). 

Then go to: 
👉 https://github.com/settings/keys 
→ New SSH key 
→ Paste it there 
→ Name it something like Enamul Laptop. 

 
 

Step 3. Change your repo’s remote from HTTPS to SSH 

Run this inside your repo: 

git remote set-url origin git@github.com:EnamulRahman/git-labs.git 
 

 

Step 4. Push again 

git push -u origin main 
 

✅ This time it should authenticate with your SSH key — no password needed. 

 

 

/ git status 

 

/ git add .filename 

 

/ git status 

 

/ git commit –m "initial commit on main"  

 

/ git checkout –b feature-1 

 

/ git push  

 

 

Fix conflicts  

 

Git Workflow: 

 

/ git pull 

/ git checkout –b feature/add-about-page 

3. / echo "sdlkglsnk" > about.md 

4. / git status 

/ git add about.d 

/ git commit –m "Add about page"  

/ git push 

/ git push –set-upstream origin feature/add-about-page 

 

Undoing in git 

 

/ git restore undo.txt  

/ unstage in git you do: git restore –-staged undo.txt 

/ git reset –-soft HEAD~1 

/ git reset –-mixed HEAD~1  

/ git reset –-hard HEAD~1 

/  

  

 

Git stash 

 

Make changes to your own work pause and come back to it 

 

/ git stash push –m "WIP"  

 

/ git stash apply – to bring it back 

/ git stash pop to remove 

 

/ git stash clear 

 

 

Git rebase and squash 

 

/ git checkout –b (go to new branch)  

Squash all commits into one 

 

/ git rebase -I HEAD~3  

 

Rebase last 3 commits  

 

 

git cherry-pick 

 

Specifically pcik 

 

97106ab  

 

Git log –oneline  for commits 

 

Git cherry-pick  

 

The “.gitignore” 

 

Sensitive info you don’t want comitted 

 

/ git amend 

 

/ git commit ---amend 

 

Pre-commit 

 

/git hooks are scrapes that run auto  check what is allowed in  

 

/ defined hooks  

 

 Install pre commit 

 
