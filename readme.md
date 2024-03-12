This is a test to see how well the GUI works from VSCode to Initialize a brand new Git Repository on Git Hub.


<br>

**Test Complete (Summary):**

So this is ~almost!~ super straight forward, except when it's not (So Close!). 

Fortunately, you don't have to do this very often. Unfortunately, the person most likely to use this guide is a newbie, who hasn't set-up Git yet in their VSCode instance.

The basic steps:
1. On your C: drive (or wherever), create an empty folder with the name of the repository you want to use in GitHub.
2. Open VSCode, and Open that Folder using Explorer.
3. Add a readme.md, and any other changes/files you want to add. (This is just so you have something to push)
4. In "Source Control" tab on the left of VSCode, select Publish to GitHub.
5. At this point I think it asks you to log into git-hub (it took my credentials so it doesn't ask me anymore for it... this might actually come later, you might have to two-factor auth as well).
6. At the top searchbar a drop down will appear for Public or Private repo.Note: If you want to change the name of the repo, **NOW** is the time to do it. Just type in the name of the repo, before selecting Public or Private.


7. If I remember it correctly, under source control, now you should be able to add a message in the top text box, and do a Commit and Push.

If you've been following along up until this point, this is where it breaks down a bit.
If this is your first time using it, it's PROBABLY going to throw an error.


If you look at the GitLog (an option on the Error Dialog box), you will see that you need to set your username and email address. At the time of this writing, I couldn't figure out how to do that from the GUI, so here we go with a few simple terminal commands.

You will need to go to the Terminal (Ctrl+Shift+`) and enter these commands. (remembering to replace your real name and email address)

`git config --global user.name "Your Name"`

`git config --global user.email youremail@domain.com`








