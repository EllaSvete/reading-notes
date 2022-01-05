## Sharing Code:

### git

- Is as sharing code and collaboration 
- Version control system 
- Let’s multiple developers work on the same code
- A history of changes to your files 
- Ability to view apply & remove - keeps changes and project files in one repository 
- Repository : space on a server, something in a file. A folder 
- It makes collaboration possible 
- What happens without version control?
- Term_paper.docx > make changes and make new versions. V1 v2 etc. we leave a paper trail 
- With git commands or “commits” = save as
- Name of doc stays same, but you can revert the document back
- Make a change from A to B without seeing A anymore. A still exists! Makes a timeline of a project. 
- Each commit has a label  that points to it. 
- HEAD= the label meaning you are here
- YOu can also assign messages to commits
- Helpful for keeping track of errors
- Head is the most recent commit
- Traceablility is important for quality
- What is Git? Vs Github?
- Git is software that uses the command line to save changes to a document. Works like a tree and nodes are added when you make commits. Creates extra bubble and keeps previous versions. Snapshots of changes, files stay the same.  Git keeps tracks of all the characters and changes and can change file system, such as reverting it back to a previous version. 
- If we are on GItHub.com we are uploading onto the github server. 
- If we’re in our terminal we are working on our machine and we have to tell github to match what local machine has. “Push command” 
- Github is industry standard for open source projects
- GIthub is like a social media so it’s a good palace to publish code and have history that hiring managers can look at. 
- Summary of Git: 
- You use git to take snapshots of your code
- Keeps a history 
- Has special label called Head”
- Usually you give a snapshot a level called a message

### GitHub:

- A Git repository (folder) in the cloud
- An online place to store code (backup is good!)
- It uses Git to help mage teams work > uses a version to connect with locally running git software
- Tracs version
- Reviews changes
- Keep changes separate until you want to add them
git(Version control)+GitHub(online code storage) = Awesome

### Repositories:

- A collection of files that you’ve told Git to pay attention to
- Usually one project = one repository 
- Really large projects might have multiple repositories (ie: front end and back end)
- Can live on Github and/or computer
- Clone :
Jacobknaack@computer 102
$ git clone (url ssh)

- $git add (makes git aware)
- $git commit -m ‘your comment’(updates files) > be specific
- $git push origin main (moves things over to the cloud)(destination)
- $remote -v origin (where you’re fetching from) shows a url

> git status : tells you what is added and what needs to be committed 
> code . 
>git add README.md : tells local git 
Git push origin main 

- How often to make commits?
The commit is you have achieved something. More commits is better than fewer commits

Git add: adds to list of files that will be changed for commit
Git status : gives you information about your current local repository 
Red things are not tracked by git
Green things are tracked and ready to commit
‘
’” is placed at the root of your repository. 
‘Git add*’ - asterisk signifies add all the changes 
Git add README.md folder/’ adds all changes starting from the paths specified
‘Git add ./’ only going to add changed going downward
Git commit: saving changes to your version history on your local machine
Git commit -m “saving photo”
Git Push: pushes “commits” or every change to GitHub
