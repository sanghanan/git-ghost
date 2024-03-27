# git-ghost

**git-ghost** is a Ruby CLI tool for managing file tracking in your local Git repository. It's all about making life a bit easier when you work with files that you don't want to push to the remote repo.

### Why git-ghost?

You know those configuration files that need to stay in the remote repo but you have to change them locally? And how annoying it is to remember not to push those changes? I love using `git add .`, but it's risky with those files around.

Normally, I'd add the file to `.git/info/exclude` and update the index to ignore changes. It's not too much work, but I thought, why not make a tool for it? Plus, I'm keen to learn more about making command-line tools with Ruby. And let's be honest, sometimes it's more fun to spend time making a tool than doing the task manually.

### Features

Here’s what **git-ghost** will hopefully let you do 🤞:

```bash
git-ghost add <file>       # Ignore a file without committing changes
git-ghost remove <file>    # Stop ignoring a file
git-ghost backup           # Backup your exclude settings
git-ghost restore          # Restore your exclude settings
git-ghost list             # Show all files you're ignoring
```

