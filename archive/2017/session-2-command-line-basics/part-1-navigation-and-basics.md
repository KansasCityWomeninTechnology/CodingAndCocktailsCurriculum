# Part 1: Navigating & Basics

---

#### Where am I?!?

The command line is just another way to navigate your computer's directory structure and issue commands. Typically, you have a **GUI**, or **G**raphical **U**ser **I**nterface, available to you. So why use a **CLI **\(**C**ommand **L**ine **I**nterface\)? Well, believe it or not, it's faster, uses fewer resources, and is much more powerful than a GUI! Let's take a look at how to orient yourself at the command line.
    {% hint style='info' %}
The terms CLI and terminal can be used interchangeably.
    {% endhint %}

When you first open your CLI, you'll likely be in your home directory at what's called a **prompt** in a **shell**. A shell is the program that provides the text-only user interface. The prompt is what's waiting on you to provide input to the shell in the form of a command. You probably will see a **~** in your CLI as well. This is a shortcut for your home directory.
    {% hint style='tip' %}
You can resize your CLI window and fonts. In Windows, right-click on the git icon at the top left of your CLI window to find the Properties menu. In iTerm2 on a Mac, there's a slew of options in the Edit and View menus.
    {% endhint %}

Let's find out what the full path to the ~ directory looks like with the `pwd` command, which stands for **p**rint **w**orking **d**irectory.
    {% hint style='tip' %}
While following along with the worksheet, type out the commands instead of doing a copy & paste to avoid inadvertently using any wrong characters.
    {% endhint %}
    
{% hint style='danger' %}
If you are using a Chromebook, please skip to the Chromebooks Only section below and expand it to follow the directions!
{% endhint %}

1. Open iTerm2 on a Mac or Git Bash in Windows.

2. Type `pwd` ![](images/enter.png) in your CLI to see your current user's home directory.
    {% hint style='info' %}
The ![](images/enter.png) icon tells you when to hit `enter`.
    {% endhint %}

3. Type `ls` ![](images/enter.png) to see the contents of your current directory.
4. Type `ls -al` ![](images/enter.png) and compare it to your previous output.  You should see more information and all files, including hidden files.
5. Next, enter in `cd CodingAndCocktails` ![](images/enter.png) to **change** **directory** into the **CodingAndCocktails** directory listed in the output of `ls`.
    {% hint style='info' %}
If the CodingAndCocktails folder doesn't exist, create it using `mkdir CodingAndCocktails`. Make sure you switch into your home folder by typing `cd ~` first. You should have done this when following [**The Tools**](https://codingandcocktailskc.gitbooks.io/coding-cocktails-the-tools/content/organization---codingandcocktails-folder.html) worksheet.
    {% endhint %}
    {% hint style='tip' %}
Both Git Bash and oh-my-zsh use formatting to distinguish between what's a directory and what's a file. You won't be able to `cd` into a file.
    {% endhint %}

6. Once you've moved into a new directory, type `ls -al` ![](images/enter.png) again to see what's listed there.
7. Let's move back up one directory. To do this, type `cd ..` ![](images/enter.png).
    {% hint style='info' %}
The **..** is a shortcut for the parent directory  much like the **~** is a shortcut for your home directory. A parent directory would be the directory that contains your current directory. No matter where you are, `cd ..` or `cd ~` are always valid commands.
    {% endhint %}

#### Tab Completion

You'll also want to utilize **tab completion** with your **tab** key and your **up/down** arrow keys. Tab completion will allow you to enter in part of a filename or directory name and then it'll be completed for you. Your up/down arrow keys will allow you to scroll through previous commands.

1. Let's switch back to the home directory by typing `cd ~` ![](images/enter.png).
2. Enter in `cd Cod` then stop and hit your `tab` key. Tab completion will find your CodingAndCocktails folder and enter the rest in for you!

Now try navigating around on your own! See the video below for some help. You can watch it in fullscreen as well. To download the video, right-click and click "Save video as...".

{% raw %}
  <video id="CLI_Part1" class="video-js" controls preload="auto" width="900" height="600"
  poster="CLI_Part1.jpg" data-setup="{}">
  <source src="videos/CLI_Part1.mp4" type='video/mp4'>
  <p class="vjs-no-js">
    To view this video please enable JavaScript, and consider upgrading to a web browser that
    <a href="http://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
  </p>
  </video>
{% endraw %}

---

<!--sec data-title="Chromebooks Only: Cloud9 Instructions" data-id="section0" data-show=true data-collapse=true ces-->

1. Sign up for an account at [c9.io](https://c9.io)
   
   Note: It will ask you for credit card information but you will not get charged for anything since we do not use features of Cloud9 that cost money. Ask a mentor for the Coding & Cocktails card for Cloud9.

2. Confirm your account from your email and log in to Cloud9.

3. Select `Workspaces` from the left side panel if you are not already there.

4. Choose `Create a new workspace`.

5. Pick a name for your workspace and enter it - it can be anything you'd like.  You do not need a description but feel free to add one if you'd like.

6. Leave your workspace as a "Public workspace".

7. In the template section choose `Node.js`

8. Click on the `Create Workspace` button.

   Cloud9 will take a minute and create your workspace here
   
9. Close the README.md file that is open when you get to your workspace.

10. In the terminal section of your workspace is where you'll be doing most of your work this evening.  If you'd like to make it bigger, hover over the top line of the terminal section with your mouse - it will change to an up-down arrow icon and then you can drag up which will also make the file editing area smaller. 

   ![](/images/c9_terminal.png)
   
11. Type `mkdir CodingAndCocktails` to created your folder/directory that you'll be working in tonight. You'll notice a new folder show up on the left side of your screen where the 
   
   {% hint style='danger' %}
Any time the worksheet mentions to change directory to your home directory or type `cd ~` you will want to type `cd ~/workspace` instead.
    {% endhint %}
    
12. Continue with Part 1 Step 1 above.


<!--endsec-->



