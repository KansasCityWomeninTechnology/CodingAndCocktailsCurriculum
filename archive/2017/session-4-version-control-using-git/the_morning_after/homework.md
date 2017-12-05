# Homework {#homework}

[![](/images/slack.png)](http://kcwit.slack.com)

1.  Think of one new tech-related term you have heard recently, and research its meaning. 

2. In Part 5 you forked the Kansas City Women in Technology Learning Resources repository from [github.com/KansasCityWomeninTechnology/LearningResources](https://github.com/KansasCityWomeninTechnology/LearningResources)

3. Open Git Bash or iTerm2 and change directories until you're in the directory for your forked Learning Resources repository. Type `cd ~/CodingAndCocktails/VersionControl/LearningResources`.

4. Configure your upstream remote (where you forked from).

   1. Type `git remote -v` to view the currently configured remotes.
   ![](/images/originRemote.png)
        
   2. Specify your upstream remote by typing `git remote add upstream https://github.com/KansasCityWomeninTechnology/LearningResources.git`
        
   3. Double check you have a new remote configured by typing `git remote -v` again.  This time you should see both origin remotes and upstream remotes. 
   ![](/images/upstreamRemote.png)

5. Fetch any new commits to the upstream repository. Type `git fetch upstream`.
        
6. Merge changes from upstream/master into your local branch.  Type `git merge upstream/master` to sync with the upstream repository without losing any local changes that you may have made.  You should now be up to date with any changes that have been committed and merged into the upstream repository since you forked the repository.

   {% hint style='info' %}
This sync only updated your local copy of the repository. To update your fork on GitHub, you must push your changes to your origin remote.
   {% endhint %}

6. Open and update the _glossary.md_ markdown document to add your term.

   {% hint style='tip' %}
Never used markdown before and need some help figuring it out? 
Check out these resources:
   1.  [help.github.com/articles/basic-writing-and-formatting-syntax](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
   2.  [guides.github.com/features/mastering-markdown](https://guides.github.com/features/mastering-markdown/)
   3.  [markdowntutorial.com](http://markdowntutorial.com/)
   {% endhint %}

5. Push your changes to your repository on GitHub.

6. Issue a pull request to the Kansas City Women in Technology repository's master branch to have your term and its definition added to our learning resources glossary.
        
7. Try this quick online interactive tutorial for a refresher! [try.github.io](https://try.github.io/)

8. If you haven't yet, take the Codecademy Introduction to Git for more practice: [https://www.codecademy.com/learn/learn-git](https://www.codecademy.com/learn/learn-git)

## Additional Resources

1.  Just for fun & more practice - Learning Git branching via a game! [http://pcottle.github.io/learnGitBranching/](http://pcottle.github.io/learnGitBranching/)

2.  The Atlassian Git Tutorial: [https://www.atlassian.com/git/](https://www.atlassian.com/git/)

3.  Pro Git Book: [git-scm.com/book/en/v2](https://git-scm.com/book/en/v2)