 Intro to Git
Version control system ( resume.pdf , resumeFINAL.pdf , resumeFinalFINAL.pdf ) Permanent record (each commit is a snapshot of the codebase at that point in time) Time machine (ability to checkout commits in history)
Parallel universes (with branches)
Mindset and approach
If your code ain't in GitHub then it doesn't exist. Push your work every day.
Add, commit, and push your work every day.
Don't worry about pushing unfinished work, just push it. Backed-up work > perfect work Write your commit messages to tell a story. What changes are here and why?
First time setup (once per project)
    1. 2. 3. 4.
5. 6. 7. 8. 9.
10.
11. 12.
13.
Open up your terminal and make sure that you're in the directory for you project. pwd shows your current directory. If necessary, navigate to the right place.
Navigate to cd ~/projects/first-repository in terminal
git init tells git to start paying attention to a folder and its contents. git init is a one
time thing per project. This command creates a local repository git status shows you all of the files that git is not yet tracking.
Do some work like create a file or change an existing file.
git add -A (this "adds" every )
git status should now show all of the files green and ready to be committed.
gitcommit-m"firstcommit".Thinkofeachcommitasasnapshotintimewitha timestamp
Navigate to https://github.com/new and create a repo. This creates a remote repository
1. Name the repo
2. Provide a description
3. Use all the defaults for readme, public, etc... 4. Click the green "Create Repository" button
BesuretousetheSSHlinkratherthantheHTTPSlink Inyourbrowser,followthedirectionsfor"...orpushanexistingrepositoryfromthe
command line"
DoublecheckthatyourworkisuponGitHub.NavigatetoyourGitHubrepoandcheckfor your work.
        
Regular process for pushing your changes (daily)
Ensure you're in your project directory cd ~/projects/first-repository
git status shows you all of the changed files, new files, and if git is tracking them.
git add hello.txt . You will use git add filename as your pattern.
git add -A will add all changes in all files to the next commit
git commit -m "This is what I am commiting and why" .
git push will upload any and all commits to GitHub (or wherever your remote is configured)
Activity
The exercise will be to create a "resources" directory on your Desktop, initialize that directory as a local git repo, save a file to this directory, and create a new remote repo in GitHub, and push your work.
Step 1 is Local
Create a directory on your Desktop named resources
Save a text from https://raw.githubusercontent.com/CodeupClassroom/git-intro/master/READ ME.md as a text file inside of resources named git-intro.md
initialize your "resources" folder as a git repository. ( git init )
git status to show the current status. The contents of the directory should be red. add the file(s) inside git add -A
git status should show the contents of the directory green now.
commit the file(s). You must commit before pushing. git commit -m "my commit message"
git status should show that everything is committed Step 2 is Remote
Go to https://github.com/new and make a new repository
Name it "resources" and provide a description like "repo for resources and notes" Click "create repository" (use the defaults for readme and the gitignore)
Step 3 is to Push your work from local to remote
Follow the directions for "...or push an existing repository from the command line"
Use this "resources" directory for any notes and extra resources. It's great git practice!
Misc
git remote -v shows any configured remotes. If this is empty, you don't have any remotes setup.
git diff shows line by line changes in your file(s). Use this prior to git add
                       