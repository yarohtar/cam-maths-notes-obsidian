This is an Obsidian Vault that I used to organize my notes on various Part IB and Part II courses. Part IB notes were created during Easter term when this project started, while Part II is being created as lectures go. 

None of this is official and it is not an accurate representation of what was lectured. I tend to give more attention to the things that I found difficult, while I might omit things that I already knew.

Most of the examples given in lectures are omitted here. 

Also the Part IB files are much more concise and probably require previous understanding of the course in order to read (because they were originally created as a revision).

You're welcome to fork this and add your own changes / notes, but if you only want to read mine, see below.

WARNING: If you clone this AND are adding your own changes AND then pulling changes from my repo, the obsidian git plugin sometimes gets very confused about merging. You should use command line git in this case. 

# How to download
Firstly, you need to download and install Obsidian from the official website https://obsidian.md/ or you can download it from the app store on your phone.

Next open the app and create a new Vault. You can delete the default file.

Go to settings (on computer, hit CTRL+, or click the gear icon on t. Go to Community Plugins. Enable them. Then click Browse and search for "Git". Install the plugin and make sure to enable it when it installs (there will be a button on the same page).

Close the Settings window(s). Hit CTRL+P to open the command palette (on windows) or click the bottom-right button and then click "Open command palette" (on android). 

Search for "Git: Clone an existing remote repo" command and hit enter.

You will be prompted a few times:
1. First enter the link to this repo, https://github.com/yarohtar/cam-maths-notes-obsidian
2. Then enter the name of a new folder where all the files will be put OR just click Vault Root
3. If asked about .obsidian file, say YES
4. If asked about merge conflicts, click DELETE
5. Leave the last prompt empty

You should be good to go now. 

# How to update from remote
If I make changes/updates to the Vault, you will be able to pull them by hitting CTRL+P and searching for "Git: Pull". This should do everything it needs to.

Alternatively, by going to Settings (CTRL+,) and clicking on Git on bottom-left, you can adjust the Autopull interval or turn on Pull on startup.

If you made changes to some files, the Pull might fail with some error messages about an impossible merge. You will either have to handle this by resolving the impossible merges (where I strongly recommend using command line git) or you'll have to reinstall the whole Vault, losing your changes.

# How to navigate
Firstly, you can switch between editing and reading mode in the top-right corner.

By hitting CTRL+O, you'll be able to search through files. Search for the course that interests you and you'll usually find an indexed file of sections / topics in that course. You can click on links to open further files (CTRL+Click to open in new tab). You can also use CTRL+J or the arrow in the top-left to navigate back.

Whenever you see a link, you can hover over while holding CTRL and it will show you a popup window of what that link is pointing to. This is useful if you just want to peak a definition and don't wanna open a new file.

In the top-left there is an Open graph view button which shows all the files / topics interconnected in a nice graph view. Can be useful to more easily figure out what's in the Vault.

Another useful feature is CTRL+P and search for links. You'll have some commands that should you outgoing links and backlinks to the current file.