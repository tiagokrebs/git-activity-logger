# git-activity-logger

I was feeling sad about moving to Bitbucket and losing my Github Profile Contribution Graph, so I made this `git` hook to register my activity using other platforms on it.

## Install
1. Create a new private repository on Github to store the activity logs and clone on local machine.

3. Copy the [pre-push](./pre-push) file to the `.git/hooks/` on the repository ou want to track contributions (Bitbucket repo) and make executable (`chmod +x pre-push`).

3. Set the necessary variables on the `pre-push` file, including the local path for the new activity logs repository you created.

## Usage
After adding the hook, every time a push is made it will register a new activity log on Github, keeping your Github contribution graph up to date. This should work to any local git repository.