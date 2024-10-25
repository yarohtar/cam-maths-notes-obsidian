This is an Obsidian Vault that I used to organize my notes on various Part IB and Part II courses. Part IB notes were created during Easter term when this project started, while Part II is being created as lectures go. 

...

None of this is official and it is not an accurate representation of what was lectured. I tend to give more attention to the things that I found difficult, while I might omit things that I already knew.

Most of the examples given in lectures are omitted here. 

Also the Part IB files are much more concise and probably require previous understanding of the course in order to read (because they were originally created as a revision).

You're welcome to fork this and add your own changes / notes, but if you only want to read mine, see below.

WARNING: If you clone this AND are adding your own changes AND are then pulling changes from my repo, the obsidian git plugin sometimes gets very confused about merging. You should use command line git in this case. 

# Courses that exist currently
Part IA:
- [[Groups]] (but taken from [[GRM]])

Part IB:
- Some [[Methods]]
- [[Optimisation]]
- [[Variational principles]]
- [[Analysis and Topology]]
- [[Quantum mechanics]]
- [[GRM]] (only [[Groups]] and [[Rings]])
- [[Numerical Analysis]]
- [[Complex Methods]]

Also useful: [[Last minute revision Part IB]]

Part II:
- [[Algebraic Topology]]
- [[Linear Analysis]]
- [[Numerical Analysis]]
- [[Asymptotic methods]]
- [[Automata and formal languages]]
- [[Principles of Quantum Mechanics]]
- Some of [[Probability and Measure]]
- Some of [[Number theory]]

# How to download
## Step 1
Firstly, you need to download and install Obsidian from the official website https://obsidian.md/ (on computer) or you can download it from the app store on your phone.

Next open the app and create a new Vault. You can delete the default file.

## Step 2

Go to settings (on computer hit CTRL+, OR click the gear icon on the bottom left; on phone swipe right and click the gear icon). 

Go to Community Plugins. Enable them. Then click Browse and search for "Git". Install the plugin and make sure to enable it when it installs (there will be a button on the same page).

Close the Settings window(s). 

## Step 3

Open the command palette (on computer you can hit CTRL+P OR find the button on the left panel; on phone you need to click the bottom right button and click "Open the command palette" OR swipe down)

Search for "Git: Clone an existing remote repo" command and hit enter.

You will be prompted a few times:
1. First enter the link to this repo, https://github.com/yarohtar/cam-maths-notes-obsidian
2. Then enter the name of a new folder where all the files will be put OR just click Vault Root
3. If asked about .obsidian file, say YES
4. If asked about merge conflicts, click DELETE
5. Leave the last prompt empty

You should be good to go now. You can see the files on the left (swipe on phone). You should probably restart the app now to sync all the settings.

Note that some things (like commutative diagrams) might not load on phone. sorry :/

# How to update from remote
If I make changes/updates to the Vault, you will be able to pull them by opening the command palette again and searching for "Git: Pull". This should do everything it needs to.

## IF it doesn't! (usually on phones)
And you get a message of type "Author not set, please do this in settings", you will need to do the following:
1. Go to Settings
2. Scroll down to Git
3. Scroll down and find fields "Author name for commit" and "Author email for commit"
4. Fill these in with your name and email

I'm not sure about the reason this doesn't work because you are never committing so this information is never actually used. But it is what it is.

## Autopull
If you don't wanna do this every time, you can set the autopull by going to Settings, scrolling down to Git and clicking on it.
Here, you can adjust the Autopull interval or turn on Pull on startup setting.

If you made changes to some files, the Pull might fail with some error messages about an impossible merge. You will either have to handle this by resolving the impossible merges (where I strongly recommend using command line git) or you'll have to reinstall the whole Vault, losing your changes.

# How to navigate
Firstly, you can switch between editing and reading mode in the top-right corner.

By hitting CTRL+O (plus icon on phone), you'll be able to search through files. Search for the course that interests you and you'll usually find an indexed file of sections / topics in that course. 

Alternatively, open this README file in obsidian and click on links in [[#Courses that exist currently]].

You can click on links to open further files (CTRL+Click to open in new tab). You can also use CTRL+J or the arrow in the top-left to navigate back.

Whenever you see a link, you can hover over while holding CTRL and it will show you a popup window of what that link is pointing to. This is useful if you just want to peak a definition and don't wanna open a new file.

In the top-left (or bottom right button on phone) there is an Open graph view button which shows all the files / topics interconnected in a nice graph view. Can be useful to more easily figure out what's in the Vault.

Another useful feature is CTRL+P and search for "links". You'll have some commands that show you outgoing links and backlinks to the current file.


