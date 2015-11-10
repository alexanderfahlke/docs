# Configuring a remote for a fork

To [sync changes you make in a fork](syncing-a-fork.md "syncing-a-fork") with the original repository, you must configure a remote that points to the upstream repository in Git.

1. List the currently configured remote repositories for your fork.

		$ git remote -v

2. Add a new remote upstream repository that will be synced with the fork.

		$ git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git

3. Verify the new upstream repository you've just specified.

		$ git remote -v
