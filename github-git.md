# Instructions for Github Classroom

> Note: The images here were produced on an OS X machine, but the same instructions (unless otherwise noted) also apply to Windows / Linux machines.

### Accessing the Assignment

Click the invitation URL provided to you by your professor.  A sample assignment for you to follow along with is provided [here](https://classroom.github.com/a/iidjEaf-).

![Github Invite Screen](images/git/github-invite-screen.png)

If you get an error message, wait a few seconds, then click `Retry Repository Setup`.  If it still fails, contact emcgee@bju.edu.  If everything works, click the URL for your new repository.

![Github Invite Finished](images/git/github-invite-finished.png)

### Cloning an Assignment Repository

To retrieve the clone URL, click the green `Clone or Download` button in the corner. 

![Github Clone](images/git/github-clone.png)

If your menu says `Clone with SSH`, click the blue `Clone with HTTPS` link to change it.  Cloning Github repositories over SSH does not work on campus.

Copy the provided url and in command prompt (or terminal), use the command `git clone <url>`.

![Github Clone Results](images/git/github-clone-results.png)

You can now make changes in the folder that has been copied to your local machine.

### Updating an Assignment Repository

After making changes, use the `git status` command to see a list of changes.

![Github Status](images/git/git-status.png)

To stage files for commiting, use `git add <filename>`.  To remove files, use `git rm <filename>`.

![Github Add](images/git/git-add.png)

Once you have the files you want to save staged, use `git commit -m "<description of what you did>"` to create a commit.

![Github Commit](images/git/git-commit.png)

Then send that commit to Github with `git push origin master`.

![Github Push](images/git/git-push.png)

You can check in the online repository browser to make sure the file made it to the server correctly.

![Github Check Commit](images/git/github-check-commit.png)

### Testing an Assignment

To test an assignment, click the `Check Submission` link at the top of the README in your repository.

If this is your first time using our testing software, you'll need to authorize the Communicator application to access your Github profile (the only information accessed is your Github username).

![Install OAuth](images/git/install-oauth.png)

After this, you will need to sign into [Jenkins](https://protect.bju.edu/cps/jenkins) with your BJU username / password.

![Login](images/git/login.png)

WARNING! Make sure that you enter your username in lowercase.  Using capital letters will cause the testing system to not recognize your login attempt and you will be denied access.

![Login Lowercase](images/git/login-lowercase.png)

Once you're at the test page, simply click `Build Now` along the right hand side.

![Build Now](images/webui/build-now.png)

In the build results, if you get a blue dot, you've passed all the provided tests.  Note that you are still advised to create your own tests as the instructor tests are much more thorough than the Jenkins tests.

![Build Now Done](images/webui/build-now-done.png)
