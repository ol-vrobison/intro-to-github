## Step 6:  Begin Work on the Story and Commit/Push a file

Move the Jira story status to “In Progress”

Create a file in home directory of the local repo, using your perfered editor, e.g. README.md and add some text to the file.

Using the Git add command, add the file to the local repo

    git add README.md

##Commit the change with a comment that starts with the Jira Ticket ID

Using the Git command line git commit -m , commit the change locally, using the Jira story id as the first part of the comment, followed by any descriptive text.  It's important to put the correct Jira ticket in the comment as this will be how all work on the story is tracked and will allow Jira integrations to display the commit information in the ticket (this will be available in Jira shortly)

    git commit -m "DDP-YYYY  Added the new README.md"

## Push the branch commit to the GitHub Repository
Using the git push command, push the branch to the repository.  The bot will wait for your push request before going on to the next step

    git push origin feature/DDP-YYYY
    