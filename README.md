# Learning_collaboration #
This is a repository to act like the main repository in a collaborative project so that I am able to simultaneously take the role of project manager and contributor.

This approach was suggested at the RLadies tutorial on GitHub


These are some of the topics I want to cover
* workflow between local repo, repo on personal GitHub account, repo on other person's GitHub account
* how to keep in sync with the main project repo

So far I think that I am getting the idea of a workflow like this
Login to your own GitHub account
Search for and go to the external account and repo that you want to contribute to
Fork a copy of the external repo to your GitHub account
## the external account should be the upstream
## the fork on your GitHub account should be the origin

Open GitBash in the directory you want your local repo to reside in
Clone a copy of your forked repo to your local directory

make a new fork for changes you want to make i.e. fix bug1 
* git checkout -b fix_bug1
* git fetch origin/master  # this is to stay upto date with any changes that have been made to GitHub repository on your account

then you  work on whatever changes you want to make in the repro

then you want to take these changes to your local repro master

* git checkout master
* git fetch fix_bug1

Check if changes are working then
Commit everything
Push the changes to your GitHub account.


Ok if you are happy with your changes you can create a pull request to the upstream repo.  But what if there are other changes to the upstream repo since you cloned the repository
on your GitHub account?  I don't see how this workflow will keep me up to date with what others are doing.

## Please Help!! ##
