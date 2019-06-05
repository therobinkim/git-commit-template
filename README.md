# git-commit-template

Write better commits by knowing when you're writing commit messages that are so long that GitHub will truncate them.

Steps:
1. Copy the contents `.gitmessage` file in this repository to a file on your machine (eg, at `~/.gitmessage`).
  a. Are you sure you want to replace any existing `~/.gitmessage` files? Check the existing contents by running the following command in your terminal: `cat ~/.gitmessage`
  b. If you're OK with creating (or overwriting an existing) `~/.gitmessage`, run the following command in your terminal: `curl https://raw.githubusercontent.com/therobinkim/git-commit-template/master/.gitmessage > ~/.gitmessage`
2. Tell Git to use `~/.gitmessage` as a template for all commit messages.
  a. Run the following command in your terminal: `git config --global commit-template ~/.gitmessage`
  b. You're done!
  
You can also enable this on a repository by repository basis by running the `git config` command from step 2a _without_ the `--global` flag from any locally cloned git repository.

You can disable this global configuration by opening your `~/.gitconfig` file in your favorite text editor and removing the `commit.template` line.
