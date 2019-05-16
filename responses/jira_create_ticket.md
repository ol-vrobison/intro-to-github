## Step 1:  Create a story in Jira

In order to meaningfully track changes in source code to software features, we will be following a branch naming convention
that identifies the Jira Story that defines the work to be done.  The convention for standard 
release development is

feature/JIRA_TICKET_ID, where JIRA_TICKET_ID is a properly formatted ticket id,
for example:

    feature/DDP-1234
    
So let's begin by creating a Jira Story for a feature

Go to Jira and create a new Story in the Dummy Development Project 
<a href="https://jira.nw.adesa.com/browse/DDP" target="_blank">Jira</a>, the return to this page for Step 2


## Step 2:  Clone your Learning Lab repository 

Using the Git command line, clone your Learning Lab repository which has already been created for you

     git clone {{ thePayload.repository.clone_url }}
Next, on the command line change directories to the newly created lab repo directory and pull the develop branch

    cd {{ thePayload.repository.name }}
    git pull origin develop
    
## Step 4: Create a Feature Branch
Using the Git command line create a branch on develop with the naming convention “feature/DDP-YYYY” where YYYY is the issue number of the Jira ticket you created

This can be done by using the git checkout -b (checkout and branch creation) 


    git checkout -b feature/DDP-YYYY 
**Be sure to use your ticket ID in place of YYYY above**    
## Step 5: Push your new branch to the Learning Lab Repository

You've created a branch on your local repository.  This branch is unknown to the remote GitHub repository  Let's push the branch so it's added to the repository
 
Using the Git command line, use the git push command to push the branch to the "origin" which is the repository source.

The Bot will wait at this step for you to complete the push, once the push is complete and the bot is notified you will be able to go on to the next step

    git push origin feature/DDP-YYYY
**Be sure to use your ticket ID in place of YYYY above**



