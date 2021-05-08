
1. Git clone
	+ git clone `<repo>`
		+ -> SSH
		+ -> HTTPS
	**eg:**
			+ https: git clone https://github.com/mhmdrahhal/testRepo.git
			+ RSA (SSH) git clone git@github.com:mhmdrahhal/testRepo.git

2. Git branch
	+ git branch `<branchname>`

3. Git commit
	+ git commit -m `<commit message>`

4. Git pull
	+ git pull origin `<branch>`

5. Git stash
	+ git stash

6. Stage changes:
	+ git add `<filename>`
	+ or git add . *(to add everything)*

7. Git checkout
	+ git checkout `<branchName>`
		+ If the branch does not exist:
		git checkout -b `<newBranchName>`
		+ If the branch exists on github but not on you PC:
			git fetch *(fetches all the branches on your repo)*
			git checkout `<branchName>`

8. Git push
	+ git push
		+ If the branch is not created on your repositry yet
			git push --set-upstream origin `<branchName>`

The flow is usually as follows:

```flow
cl=>start: Clone
wk=>operation: Change filed
ad=>operation: Stage changes
cmt=>operation: Commit changes
ps=>end: Push your changes

cl->wk->ad->cmt->ps

```


