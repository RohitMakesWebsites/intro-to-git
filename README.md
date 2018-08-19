### Table of Contents

* [Importing your Assignment into Eclipse](https://github.com/WilcoxAPCS/intro-to-git/blob/master/README.md#importing-your-assignment-into-eclipse)
* [Uploading your Changes to Github](https://github.com/WilcoxAPCS/intro-to-git/blob/master/README.md#uploading-your-changes-to-github)
* [Understanding GitHub](https://github.com/WilcoxAPCS/intro-to-git/blob/master/README.md#understanding-github)

### Importing your Assignment into Eclipse


1. Open **Eclipse**, File > Import

![](https://i.imgur.com/GEbQ2yp.png)

2. For `Select`, Select Git > Project from Git > Next

![](https://i.imgur.com/SbN0yI5.png)

3. For `Select Repository Source`, Select Clone URI > Next

![](https://i.imgur.com/MvYmksp.png)

4. For `Source Git Repository`, enter the following:
   - URI: `https://github.com/WilcoxAPCS/introduction-to-github-username`. This should autopopulate the Host and Repository path field. Remember to substitute your own username in!
   - Your username and password for Github in the Authentication section, then Next.

![](https://i.imgur.com/m06kdX7.png)

5. For `Branch Selection`, master should automatically selected, then just hit Next.

![](https://i.imgur.com/MhndBev.png)

6. For `Local Destination`, a directory will be auto-populated for you, feel free to change this if you wish, otherwise Next.

![](https://i.imgur.com/d1sq9rW.png)

7. For `Select a wizard to use for importing projects`, make sure Import existing Eclipse projects is selected, then Next.

![](https://i.imgur.com/IOQDll5.png)

8. On the `Import Projects` menu, you should see the HelloWorld Project. Make sure it is selected and you're done! Hit Finish

![](https://i.imgur.com/FZ2shlD.png)

9. You should now be able to see your new project in the `Package Explorer`. If you cannot see your Package Explorer. Window > Show View > Package Explorer.

![](https://i.imgur.com/XDIWEoK.png)

### Uploading your Changes to Github

1. Right click on your project. Team > Commit

![](https://i.imgur.com/e9yVloi.png)

2. The `Git Staging` panel will open. Move any changes you want to commit from **Unstaged Changes** to **Staged Changes** by selecting the item, and clicking the green plus.

![](https://i.imgur.com/tG42ZEF.png)

3. Once you have staged everything your heart desires, add a commit message ([this usually describes what your changes do](https://chris.beams.io/posts/git-commit/)). For Author and Commiter, put `username <email@email.com>`, replacing with your username and email of course. Commit and Push!

![](https://i.imgur.com/kYYzvwI.png)

4. You will be prompted to log in, so Github knows who is making the changes. You should be able to see your changes on your page after this!

![](https://i.imgur.com/L8j6id4.png)

### Understanding GitHub

For class, you can simply follow the instructions above to import and submit your assignments. This section is additional reading for those interested in developing a deeper understanding of Git and the terminology used in the above sections.

**_What is Git?_**

Git is a version control system for tracking changes in computer files and coordinating work on those files among multiple people. The terminology you have seen in the instructions above (i.e. repository, branch, remote, commit, staged, push) is Git terminology. Version control allows us to easily maintain versions of our code, and collaborate with others.

**_What is GitHub?_**

GitHub is a website where you can upload a copy of your Git repository. It is a Git repository hosting service, which offers all of the distributed revision control and source code management functionality of Git as well as adding its own features. GitHub Classrooms, which is what we are using is one of GitHub's additional features. It is also a standard platform to show off your coding projects!

**_How does it work?_**

We will use this coding assignment as an example.

When you accepted the assignment, a private GitHub private remote repository was created for you, hosted on GitHub. Using Eclipse as an interface, we fetched a local copy of the repository from the host. 

This local Git repository will track your changes, allow you to make commits, and push to the back to the remote repo (the version seen on Github)

![](https://qph.fs.quoracdn.net/main-qimg-3aa29f29ede6a8245b6964f663c60339.webp)

Terminology | Description 
--- | --- 
Working Directory | The directory in which you are currently working (i.e. What you are seeing in Eclipse as right now). 
Staging Area | A place to put all the files you want to commit
Local Repo | Your local version of the repository.
Remote Repo | The hosted version of the Repository

Note: In the use case of a private repository where you're working alone, it might not be immediately obvious why we have both a local and a remote repo. *Why not commit straight to remote?* This is because in real life scenarios, there are many cases where you want your local repository changes to be approved before you push to the published remote repo. Another feature often used is branches, which we will not cover as we will simply use the `master` branch, but more information about branches can be found [here](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell).

In Eclipse, when we used the green plus to move Unstaged Changes to Stage changes, it is using the `add` function to move our changes from our working directory to our staging area. Then when 'Commit and Push' was pressed, the `commit` command was used to push changes from our staging area changes to our local repository immediately followed by a `push` command to push our local repository changes to our remote (so we can view our changes on GitHub!).  

The functionality of Git is incredibly rich, and there is much more to learn beyond what is covered here. A list of additional functionality is available on [this page](https://git-scm.com/docs), for those looking to learn more.
