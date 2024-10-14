This is an Obsidian Vault that I used to organize my notes on various Part IB and Part II courses. Part IB notes were created during Easter term when this project started, while Part II is being created as lectures go. 

None of this is official and it is not an accurate representation of what was lectured. I tend to give more attention to the things that I found difficult, while I might omit things that I already knew. 

You're welcome to fork this and add your own changes / notes, but if you only want to read see 

WARNING: If you clone this and add your own changes, and then pull changes from this repo, the obsidian git plugin sometimes gets very confused about merging. You should use command line git in this case.

# How to download
Firstly, you need to download Obsidian from the official website https://obsidian.md/

Next open the app and create a new Vault. You can delete the default file.

Go to settings on the bottom left (alternatively, hit CTRL+,). Go to Community Plugins. Enable them. Then click Browse and search for "Git". Install the plugin and enable it. 

Close the Settings window(s). Hit CTRL+P to open the command palette. Search for "Git: Clone an existing remote repo" and hit enter.

You will be prompted 3 times:
1. First enter the link to this repo, https://github.com/yarohtar/cam-maths-notes-obsidian
2. Then enter the name of a folder (can be the same as the name of the Vault)
3. Leave the third prompt empty and hit enter

You should be got to go now. 

# How to update from remote
If I make changes/updates to the Vault, you will be able to pull them by hitting CTRL+P and searching for "Git: Pull". This should do everything it needs to.

Alternatively, by going to Settings (CTRL+,) you can 

If you made changes to some files the Pull might fail with some error messages about an impossible merge. You will either have to handle this by resolving the impossible merges (where I strongly recommend using command line git) or you'll have to reinstall the whole Vault, losing your changes.