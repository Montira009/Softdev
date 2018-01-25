# Softdev


# Branch
	$ git branch yourbranch 		// Create Branch
	$ git checkour yourbranch		//Move to branch yourbranch
	$ git checkout -b yourbranch 		//Create branch and move to new branch
	$ git branch -a 			// Status branch
	$ git branch -d yourbranch 		//Delete branch | Move to master first.
	$ git push -u origin yourbranch	


# -- Upload branch to master --
	$ git checkout master
	$ git merge --no-ff dev 		// merge dev to master | --no-ff 