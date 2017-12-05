### Part 6: Branching and the Art of Collaboration {#part-6-branching-and-the-art-of-collaboration}

Now we are going to collaborate on a very simple web application.

1.  In Google Chrome, navigate to [https://github.com/KansasCityWomeninTechnology/DrinkOrderApp](https://github.com/KansasCityWomeninTechnology/DrinkOrderApp). 

2. Click on the issues tab at the top.

3. Look through the list of issues for one that does not yet have a comment icon on the right side: ![](/images/comment.png)

4. Click on the issue to open it and at the bottom, add a comment saying the issue is assigned to you.  For example,  "This issue is assigned to @codingandcocktails." Replace codingandcocktails with your own GitHub username, leaving the @ symbol to tag yourself. Make note of the issue number to use in step 8. 

    {% hint style='info' %}
You may see development teams assign work via the "Assignee" option on the upper right corner of the issue.

![](/images/assignment.png)

We are not using that option to simplify user management tonight.
    {% endhint %}

5. Fork the repository.

    {% hint style='tip' %}
If you need a refresher on how to fork a repository go back to [Part 5: Forking](/class_exercises/part_5_practice_with_forking.md).
    {% endhint %}

6. In Git Bash or iTerm2 make sure you are in your _VersionControl_ directory.  If you are anywhere else change directories to the _VersionControl_ directory.

7. Clone the forked repository and `cd` into it.

8. Using the issue number from step 4, we will now make a new branch. In Git Bash or iTerm2, type `git checkout -b issue-##` to do this replacing ## with your issue number.

    {% hint style='tip' %}
If you are working on issue #9, your branch name would be **issue-09**.
    {% endhint %}

9. To view all branches within the repo, type `git branch` . This should show you at least two branches - master, and the issue-## branch you just created. The branch you are currently working in will be highlighted with an asterisk (*).

    {% hint style='tip' %}
To switch between branches type `git checkout branchname` replacing the text "branchname" with the branch you'd like to switch to.  For example if you want to switch to the "development" branch you'd type `git checkout development`.
    {% endhint %}
    
10.  In Git Bash or iTerm2 type `atom .`. This will open your Atom text editor with the context of the current directory.

11. Make changes to the application as instructed in your issue and make sure to save any files you change. 

12.  After you've saved your files, in Git Bash or iTerm2, type `git status` to view which files you've changed. 

13. If everything looks good, stage and commit your changes. Type `git push origin <branchname>` to push to the branch you made to your remote fork, substituting your own branch name for the angle brackets and "branchname" text. Now you have pushed your changes to the _origin_ (that is, to the cloud), to your specific branch.

14. Create a **pull request** to migrate your changes from the fork and branch you have been working on to the Kansas City Women in Technology repository.

    1. In Google Chrome, navigate to [https://github.com/KansasCityWomeninTechnology/DrinkOrderApp](https://github.com/KansasCityWomeninTechnology/DrinkOrderApp) and click on the **New Pull Request** button.
    
    ![](/images/pullrequest.png)

    2. Click the "compare across forks" link at the end of the text "Compare changes across branches, commits, tags, and more below. If you need to, you can also compare across forks."
    
    3. Keep the "base fork" (organization where you are moving your changes **TO**) as KansasCityWomeninTechnology 

     4. Change the "base" (the branch within the organization you selected to move your changes **TO**) as "vc-final".
    
    5. Change the "head fork" (User that you're moving changes **FROM**) to yourGitHubusername/DrinkOrderApp 
    
    6. Change the "compare" to the issue-## branch you created in step 8.
    
    Feel free to add any comments you'd like.  If you keep scrolling down you'll see the commits you added to make the change along with the diff across the file(s) you changed.
    
    5. Click on the Green "Create pull request" button.

    {% hint style='info' %}
If Git detects no conflicts, it will give you a checkmarked message saying “able to merge.”

![](/images/mergeable.png)
    
If Git detects conflicts, it will display a red message saying "Can't automatically merge."

![](/images/cantMerge.png)
    {% endhint %}

15.  Typically someone or a group of people have oversight into merging the pull requests into the upstream repository (where you forked from) to become the final version of the code. Once your pull request is accepted by this person, you can view your code in the final destination, along with all of the changes your peers have made.

    We will work on getting PR's (aka Pull Requests) merged as we are able!

**Congratulations! You’ve collaborated on a project for the first time!**