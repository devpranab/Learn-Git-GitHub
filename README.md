Prepared by devpranab

<body>
    <h1>Learn Git & GitHub -by pranav</h1>
    <img src="https://i.ibb.co/q9xGjDp/git-workflow.png" height="170px" alt="git-workflow" border="0">
    <!-- Docs link -->
    <a href="https://git-scm.com/doc">Docs link</a>
    <h2>Version Control System</h2> 
    <p>Git/SVN/CVS</p>
     <p>GitHub/GitLab/GitBucket</p>
    <h3>Softwere Tool to manage changes to source code over time, It keeps track of every modification to the code</h3> 
    <h4>Installing Git on pc (git-scm.com) :</h4>
<pre>right click on Desktop > Git Bash Here > git --version - check git
veriable setup: git config --global user.name "Pranav Sarkar"
                git config --global user.email "spranab654@gmail.com"
                git config --list - check veriable setup
    </pre>
    <h4>Using basic Git Commands :</h4>
<pre>
    >ps - command line name
    >ls - what have in this folder
    >ls -lart - show files
    >mkdir folder - create this folder
    >rmdir folder - remove this folder
    >touch test.js - create this file
    >cat test.js - show open this file
    >cd js - change directory
    >cd 'js master' - change directory
    >cd .. - back 1 folder
    >cd\ - back root folder
    >cd ../ - back root
    >start chrome index.html - open in browser
    >clear
    >pwd - current path show
    >Q - press for back terminal
</pre>    
    <h4>Use Git in Project Development :</h4>
<pre>
    >git init - init git in your project
    >git status - current status check
    >git add test.js - tracked this files
    >git add folder/test.js - tracked this files
    >git add . - tracked all files in folder
    >git add * - tracked all files in folder without deleted file
    >git add *.txt - tracked all .txt files in folder without deleted file
    >git add -A or git add --all - tracked all folders
    >git rm test.txt - remove this file
    >git rm test.txt -f - remove this file
    >git rm --cached test.txt - opposite of -f
    >git rm -r folder - remove recursively
    >git reset - all reset
    >git reset test.js - untracked this file
    >git reset --hard - reset from staged folder
    >git reset HEAD hot.txt - reset from staged folder
    >git checkout test.js - back file
    >git checkout -f - back files
    >git diff - show dff after edit before commit(local stage compare)
    >git diff --staged - stage-last commit compare
    >git diff 04496d4 3fg88c6 - two commit compare
    >git commit -m "first commit" - checkpoint commit
    >git log --stat -M - show all commit logs with indication of any paths that moved
    >git reset HEAD~ - commit rollback
    >git log - show all commit
    >git log --oneline - show all commit
    >git log -p -1 - show last commit
    >git log -p -2 - show last two commit
    >git log --oneline - show all commit
    >git checkout 4ee2e80 - switch on this checkpoint
    >git checkout 4ee2e80 test.js - switch on that checkpoint
    >git checkout -- - leatest version
    >git branch -M main - keep project in branch
    >git remote add origin https://github.com/devpranab/em-john-MERN.git - github remote location
    >git push -u origin main - project upload
</pre>
<h4>Fetch & Pull :</h4>  
<pre>
    <!-- fetch or pull -->
    >git fetch
    .git merge
    or
    >git pull - bring code from repo into vs code
</pre>
<h4>Pull Request on GitHub :</h4>
<pre>
Another Developer worked in another brnch & he can propose to add her code
</pre>
<h4>Fork :</h4>
<pre>
bring project from another Github a/c and keep at your repo by fork
 >click repo > fork > 
</pre>
<h4>Stash & Clean :</h4>
<pre>
for change code keeping old code
 >git stash - hide
 >git stash pop/git stash apply - last stash return
 >git stash list - all return/show
 >git stash pop stash{0} - switch on that stash
 >git stash pop stash{1} - switch on that stash
 >git clean -f -n - remove alert
 >git clean -f - removed
</pre>
<h4>About .gitignore file :</h4>
<pre>
    >touch .gitignore - keep untracked,uncommit file
    -app.js - file
    -/css - folder 
</pre>
<h4>Branch & Merge :</h4>
<pre>
    >git branch - show all branch
    >git branch oneTask - create oneTask branch
    >git branch -d oneTask - delete oneTask branch
    >git checkout oneTask - switch to oneTask branch
    >git add .
    >git commit -m - commit on oneTask branch
    >git merge oneTask - merge with oneTask(master)
    >git merge oneTask -m "conflict" - merge with oneTask(master)
    >git checkout oneTask
    >git push -u origin oneTask - upload oneTask branch to
    >git rebase [branch] - apply any commits of current branch ahead of specified one
    
    <!-- merge conflict problem -->
</pre>
<h4>NPM using Git Commands :</h4>
<pre>
    >npm init or npm init --yes
    >npm i bootstrap - installing this npm package
    >npm i bootstrap@5.1.0 - installing this npm package with this version
    >npm un bootstrap - uninstalling this npm package
</pre>
<h4>Host GitHub Repo :</h4>
<pre>
open repo > create new branch(gh-pages) > settings > GitHub Pages-check it out > copy this link
</pre>
<h4>Clone from online Git Repos in VS Code :</h4>
<pre>
code > copy HTTPS link > open vs code > git icon sidebar > clone repository > paste above
or
git clone link
git clone link name
</pre>
<h4>SSH Key Generate :</h4>
<pre>
GitHub id,password alert turn off:
Credential Manager > Windows Credential > Generic Credential > git:https://github.com - Remove
 >ssh-keygen -t rsa -b 4096 -C "spranab654@gmail.com"
 >git_keys
 >password
 >again password
 >eval $(ssh-agent -s)
 >ssh-add ~/.ssh/id_rsa
 >password
 >clip < ~/.ssh/id_rsa.pub
 Add this on GitHub:
 GitHub > SSH and GPG keys > New SSH Key > Title,Key -here paste ssh key
 Add SSH key > Now select SSH in repo > Now push without email,password
 >git remote add origin https://github.com/devpranab/em-john-MERN.git
 >git push -u origin main
</pre>
<h4>Using online Git Repositories(GitHub Desktop) :</h4>
<pre>
Download GitHub Desktop > 
</pre>

<h5>Default Terminal -settings.json</h5>
<pre>
   "terminal.integrated.defaultProfile.windows": "bash",
   "terminal.integrated.shell.windows": "C:\\Program Files\\Git\\bin\\bash.exe"
</pre>
<img src="https://i.ibb.co/0BDyxht/git-cheat-sheet-large.png" alt="git-cheat-sheet-large" border="0">
<hr/>
<h2>Git Error Fixing :</h2>
<pre>
01. PROBLEM: $ git push -u origin main
To https://github.com/devpranab/MongoDB-Learn.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/devpranab/MongoDB-Learn.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
SOLUTION:
$ git fetch origin main:tmp
$ git rebase tmp
$ git push origin HEAD:main
</pre>
</body>
