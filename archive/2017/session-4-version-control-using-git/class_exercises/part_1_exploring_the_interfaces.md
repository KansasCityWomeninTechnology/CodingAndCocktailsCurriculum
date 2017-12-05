### Part 1: Exploring the Interfaces {#part-1-exploring-the-interfaces}

1.  If you use Windows, open Git Bash, or if you use a Mac, open iTerm2.

2.  Type `cd CodingAndCocktails` to navigate to your `CodingAndCocktails` directory in your home directory.

    {% hint style='tip' %}
If you don't have a CodingAndCocktails directory created refer back to [The Tools instructions](https://codingandcocktailskc.gitbooks.io/coding-cocktails-the-tools/content/organization---codingandcocktails-folder.html) to create it.
    {% endhint %}

3. Type `mkdir VersionControl` to make a new folder for this month. Then type `cd VersionControl` to move into that folder.

    {% hint style='tip' %}
For a refresher on command line, check out the worksheet from last month: [bit.ly/CnCMarWork](http://bit.ly/CnCMarWork).
    {% endhint %}

3.  Type `mkdir GUIRepo` to make a new directory inside your  VersionControl directory. Your directory structure should now look like this:
```
CodingAndCocktails
        |
        |--VersionControl
                |
                |--GUIRepo
```
4. Type `git gui`. This will open the GUI (Graphical User Interface) to interact with Git.
    ![](/images/gitgui.png)

5. Click **Create New Repository** and **Browse** to your _GUIRepo_ directory and choose it.

6. Click **Create** This will turn _GUIRepo_ into a Git repository and bring up the GUI , which you may explore but we will not go into detail in class.

7. To return to the command line either:

    a) Exit out of Git GUI the same way you exit out of any program, or 
    
    b) In iTerm2 or Git Bash, press the `ctrl` + `c` keys on your keyboard to return to your command prompt.
    
8. In Google Chrome, navigate to [Github.com](github.com) and log into your account. Take a look around.  View your profile by selecting that option from the drop down menu in the upper right.  This will be more exciting to look at once we have a bit more GitHub interaction. 

You just created your first repository using the Git GUI and explored GitHub - your cloud storage area for your repositories.  

{% hint style='info' %}
Since most people are more familiar with computer interaction via some sort of graphical user interface, we wanted to first introduce that option since it might be a bit more comfortable in addition to making you aware that there are multiple ways to interact with Git.

However, most development teams don't use the GUI because it becomes faster to interact with Git via the command line once you've had additional practice and are more comfortable. 
{% endhint %}
