# Syncing a fork

Before syncing a fork with an upstream repository, you have to [configure a remote that points to the upstream repository](configuring-a-remote-for-a-fork.md "configuring-a-remote-for-a-fork") in Git.

1. Fetch branches and their commits from the upstream repository. All commits to ```master``` from the upstream repository will be stored in a local branch named ```upstream/master```.


		$ git fetch upstream

2. Check out your fork's local ```master``` branch.

		$ git checkout master

3. Merge the changes from ```upstream/master``` into your local ```master``` branch. This will syncronize your fork's ```master``` with the upstream repository. You don't loose local changes.

		$ git merge upstream/master
