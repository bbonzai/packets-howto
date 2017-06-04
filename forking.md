## How to fork a repository and then merge your fork ##

### What is a fork? ###

When you make modifications to *some other user's* repository, you are 
said to be `forking` it.

After you've forked someone's repo and made modifications to its contents, 
then you *may* request that your fork should be incorporated into the 
original user's repo.  If that user chooses to incorporate it into the
"master" branch of his repo, then you have made a permanent contribution
to that repo.  (Since `git` tracks modifications to any repo, your
change could, in principle be undone; but once your change is incorporated
into the `master` branch of the original repo, it has become a "standard" 
part of that repo.

### How to start a new fork ###

Visit the repo of the project you wish to fork.  Suppose you want to 
fork the repo `microcontrollers.intro` of the user `RoboticsAndBeyond`.
Then, in your web browser, visit:

    https://github.com/RoboticsAndBeyond/microcontroolers.intro

Initiate the fork:  near (but not at) the upper right corner, 
click on the icon for a fork:  <svg height="28.000029"
   class="octicon octicon-repo-forked"
   viewBox="0 0 9.9965315 14.000014"
   version="1.1"
   width="19.993063"
   aria-hidden="true">
  <path d="M 7.998266,6.9569837e-6 A 1.993,1.993 0 0 0 6.998266,3.720007 v 1.28 l -2,2 -2,-2 v -1.28 A 1.993,1.993 0 0 0 1.998266,6.9569837e-6 1.993,1.993 0 0 0 0.99826595,3.720007 v 1.78 l 3.00000005,3 v 1.78 a 1.993,1.993 0 0 0 1,3.72 1.993,1.993 0 0 0 1,-3.72 v -1.78 l 3,-3 v -1.78 a 1.993,1.993 0 0 0 -1,-3.7200000430163 z M 1.998266,3.200007 c -0.66,0 -1.20000005,-0.55 -1.20000005,-1.2 0,-0.65 0.55000005,-1.20000004 1.20000005,-1.20000004 0.65,0 1.2,0.55000004 1.2,1.20000004 0,0.65 -0.55,1.2 -1.2,1.2 z m 3,10 c -0.66,0 -1.2,-0.55 -1.2,-1.2 0,-0.65 0.55,-1.2 1.2,-1.2 0.65,0 1.2,0.55 1.2,1.2 0,0.65 -0.55,1.2 -1.2,1.2 z m 3,-10 c -0.66,0 -1.2,-0.55 -1.2,-1.2 0,-0.65 0.55,-1.20000004 1.2,-1.20000004 0.65,0 1.2,0.55000004 1.2,1.20000004 0,0.65 -0.55,1.2 -1.2,1.2 z"
     id="path2"
     style="fill-rule:evenodd" /></svg>

This action sets up a copy of the original (aka "upstream") repo in your account.

### How to make modifications within your new fork ###

Navigate to the new cloned repo that you just set up.  Let's say your account name is `bbonzai`.
Then the new repo would be accessed at:

    https://github.com/bbonzai/microcontrollers.intro

Set up a new branch.  You will make your changes in that new branch.  To do this,
click on the drop-down menu labelled "Branch", and fill in a short name for your new branch.
Suppose you decide to call it `FixMetaData`.  Make sure that branch is selected in the
Branch pull-down menu before your next step.

Navigate to whichever file you want to change, e.g. `Projects/Laser_Tag/circuit.md`.
Click on the pencil icon to the top right of the window where this file's contents appear
to start editing it.  

After you've finished your edits, scroll down to below the editor window, and find a
window labelled "Commit changes".  Enter a short comment describing your change; in this case,
the comment is "Removed metadata".  Then click the green button "Commit changes".

### Request that your modifications be incorporated into the upstream repo ###

Go back to the top level of your fork:

    https://github.com/bbonzai/microcontrollers.git

Ensure once again that the correct branch is selected in the Branch pull-down menu.
In this case, it should be `FixMetaData`.  Then click the button labelled `New pull request`.
You are now about to ask the *owner* of the original upstream repo to pull your changes
into his repo.   

GitHub will check whether your changes can be merged into the upstream repo without
any conflicts.  If so, you'll see a screen that says (in green) "Able to merge".
You will find a box where you should make a comment (to the owner of the repo) saying
why he should incorporate your modifications.  Then click the green button "Create pull
request".  At that point, you'll have to wait til the owner of the upstream repo reviews
and responds to your request.

### What happens after your changes were received by the upstream repo owner ###

The owner may:

* *agree* to incorporate your modifications, in which case he will merge them
into the `master` branch.

* *reject* your modifications, in which case he will send you a message explaining
his rationale.

If you wish, you can now destroy your fork.  To do this, visit your account; in this 
case:  `https://github.com/bbonzai/microcontrollers.intro`.
Then click on the `Settings` tab, navigate to the bottom of the page (labelled "Danger Zone")
and click on the button that says "Delete this repository".  You'll see a pop-up window 
where you must enter the exact name of your repo (in this case `microcontrollers.intro`),
and then click a button claiming you understand the consequences of this removal.    
