This is a test to see how well the GUI works from VSCode to Initialize a brand new Git Repository on Git Hub.


<br>

**Test Complete (Summary):**

So this is *almost* super straight forward, except when it's not (it's So Close!). 

Fortunately, you don't have to do this very often. Unfortunately, the person most likely to use this guide is a newbie, who hasn't set-up Git yet in their VSCode instance.

The basic steps:
1. On your C: drive (or wherever), create an empty folder with the name of the repository you want to use in GitHub.
2. Open VSCode, and Open that Folder using Explorer.
3. Add a readme.md, and any other changes/files you want to add. (This is just so you have something to push)
4. In "Source Control" tab on the left of VSCode, select Publish to GitHub.
5. At this point I think it asks you to log into git-hub (it took my credentials so it doesn't ask me anymore for it... this might actually come later, you might have to two-factor auth as well).
6. At the top searchbar a drop down will appear for Public or Private repo.Note: If you want to change the name of the repo, **NOW** is the time to do it. Just type in the name of the repo, before selecting Public or Private.
7. Select which files to include in the initial push by checking the box.


If you've been following along up until this point, this is where it breaks down a bit. 

- If you already had Git Set-up, and your Git-Hub logged on, VSCode probably succeeded, and created a new repository in GitHub, with either the name you chose, or the name on the file folder.

- If this is your first time using it, it's *PROBABLY* going to throw an error.

<br>
<br>
** Fix #1 **

If you get the error, and then look at the GitLog (an button on the Error Dialog box should take you there), you will see that you need to set your username and email address. At the time of this writing, I couldn't figure out how to do that from the GUI, so here we go with a few simple terminal commands.

You will need to go to the Terminal (Ctrl+Shift+`) and enter these commands. (remembering to replace your real name and email address)

`git config --global user.name "Your Name"`

`git config --global user.email youremail@domain.com`


<br>
<br>
** Fix #2 **

If you get the error, the whole process *probably* aborted... which means, it never created the "Remote" connection in the configuration. To do that manually, in the Source Control tab again, there is a section called "Remotes".

1. Hit the Plus sign (Add Remotes).
2. At the top in the search box, give it a name (usually 'origin' by default)
3. Next give it the full URL to the git-hub repository. (https://github.com/kohlmann0/GitTest as in this example)


<br>
<br>
** Fix #3 **
Last but not least, if the process aborted originally, it probably didn't finish the commit, and probably didn't push the code changes. To do that...

1. Save any file changes you may have made (for example, editing this .md file)
2. At the top of the Source control box, give it a commit message. **Do Not Hit Commit Yet!** (that's for all the new people).
3. Under "Changes" hit the Plus sign (Stage Changes) for whatever file you want to Commit and Push.
4. It's somewhat frowned upon to "Commit and Push" in one step, *especially* to the master branch, but just for the sake of finishing this summary off fast... "Select Commit & Push" from the drop down, and it ***SHOULD*** push all of your staged changes directly to your shiny new Git-Hub Repository.


Once you've done these three fix's for your first project, everytime after that should run super smooth. It's just getting that initial set-up straight. Even on other projects, it should "Just Work" once you've done the first one. 

Check back later when I create a Docker Container Dev environment in a new repository.






