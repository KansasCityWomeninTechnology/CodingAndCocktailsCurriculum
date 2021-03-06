# Prep Work

{% hint style='danger' %}
If this is your first time joining us for Coding & Cocktails, you'll want to [install our tools](http://bit.ly/CnCTheTools) before you go any further.
{% endhint %}

### 1. <a href="https://kcwit.slack.com/messages/C0BGBKGG6">Click Here to Open Slack</a>

If you have a tip that helped you with a step on the worksheet, you can easily share it with the group in Slack. Or if there are any issues with the worksheet [we make typos or there's an update to a tool that we didn't catch before the session], we may post updates in Slack. Plus, after class is over, Slack becomes a tool for you to gain access to mentors as you go through the homework, or any other questions that arise.

### 2. Install/Update Node.js & npm

{% hint style='danger' %}
If you're using a Chromebook, skip down to the Cloud9 instructions at the bottom.
{% endhint %}

{% hint style='danger' %}
If you joined us earlier this year, you might have installed Node.js & **npm**, but you'll still want to update to the latest version of Node.js & **npm**.
{% endhint %}

1.  Open Git Bash or iTerm2

  {% hint style='info' %}
  The "terminal" and "command line" (aka CLI, command line interface) are the same thing.
  - On Windows, we use **Git Bash**
  - On Mac, we use **iTerm2**
  {% endhint %}

2.  In your CLI, type: `node --version`

    1. No version number [something like `node: command not found`]. You need to install Node.

      <!--sec data-title="Mac - Install Node" data-id="sectionInstallMac" data-show=true data-collapse=true ces-->

      1. In iTerm2, type: `brew update`

      2. When that finishes, type: `brew install node`

      3. Confirm `node --version` returns a version **8 or greater**.

      <!--endsec-->

      <!--sec data-title="Windows - Install Node" data-id="sectionInstallWindows" data-show=true data-collapse=true ces-->

      1. [Download](https://nodejs.org/en/) the **Current** installer for Windows.

      2. Double-click on the downloaded file & follow the installation prompts.

      3. When that finishes, confirm `node --version` returns a version **8 or greater**.

      <!--endsec-->

    2. If your version number is **8 or greater**, proceed to Step 3.

    3. If your version number is less than **8**, you'll need to update Node.

      <!--sec data-title="Mac - Update Node" data-id="sectionUpdateMac" data-show=true data-collapse=true ces-->

      1. In iTerm2, type the following: `brew update`

      2. When that finishes, type: `brew upgrade node`

      3. Confirm `node --version` returns a version **8 or greater**.

      <!--endsec-->

      <!--sec data-title="Windows - Update Node" data-id="sectionUpdateWindows" data-show=true data-collapse=true ces-->

      1. [Download](https://nodejs.org/en/) the **Current** installer for Windows.

      2. Double-click on the downloaded file & follow the installation prompts.

      3. When that finishes, confirm `node --version` returns a version **8 or greater**.

      <!--endsec-->  

3. Let's check your version of **npm** [which was installed with Node]. [_Version **5 or greater** required._]  
   In your CLI, type: `npm --version`  

   1. If your version is **5 or greater**, proceed to Step 3.

   2. If your version is less than **5**, update to the latest by typing: `npm install npm -g`

### 3. Install angular-cli

1.  In Git Bash (windows) or iTerm2 (macs), type: `npm install -g @angular/cli`

 *This may take a minute or two to complete. Perfect excuse to grab yourself a drink!*

2.  To confirm Angular CLI was installed, while still in Git Bash or iTerm2, type: `ng version`. If you get a version number, you can move on!

    ![](/images/ngVersion.png)

### 4: Add TypeScript Package to Atom

Using TypeScript with Angular2, provides us a lot of shortcuts. However, to make sure the correct words highlight for us in Atom (maybe you've noticed the colors in HTML, CSS or JavaScript files?), and that we get some of the autosuggest features of TypeScript, we have to install the TypeScript package for Atom.

1.  Open Atom and from the Atom menu and choose **Preferences** (mac) or File menu and choose **Settings** (windows).

2.  In the Preferences pane click on the **Install** option. 

    ![](/images/install.png)

3.  In the search bar, type **Typescript**

4.  Find & select the TypeScript package that matches this image:

    ![](/images/typescriptPackage.png)

    {% hint style='info' %}   
If you are prompted to install any dependencies select **Yes** to install them.
    {% endhint %}

6. Hover over the settings tab at the top of the page and an x should appear.  Click the x to close the settings tab.

7. Setup is done! Give high fives to those around you!

<!--sec data-title="Chromebooks Only: Cloud9 Instructions" data-id="section0" data-show=true data-collapse=true ces id="chromebook"-->

1. Sign up for an account at [c9.io](https://c9.io)

  Note: It will ask you for credit card information, but you will not get charged for anything since we do not use features of Cloud9 that cost money. Ask a mentor for the Coding & Cocktails card for Cloud9.

2. Confirm your account from your email and log in to Cloud9.

3. Select **Workspaces** from the left side panel if you are not already there.

4. Choose **Create a new workspace**.

5. Add a name for your workspace - it can be anything you like. You do not need a description, but feel free to add one if you like.

6. Leave your workspace as **Public**.

7. In the template section select the Node.js option.

8. Click on the **Create Workspace** button.

  Cloud9 will take a minute and create your workspace here.

9. When the workspace opens, click on the small x on the right side of the tab that says `[M]/README.md` to clear your workspace.

10. On the left side project pane, right click on the _client_ folder choose **Delete**.  Then confirm Yes you want to continue. Repeat for the _package.json_, _README.md_, and _server.js_ files.  

9. We need to update the version of Node.js that Cloud9 uses by default. We'll use a tool called **Node Version Manager** to use version 8. In the terminal section of your workspace (that's the bottom portion with the `~/worspace $` prompt), type: `nvm install 8`

  ![](assets/images/c9_terminal.png)

 {% hint style='tip' %}

 To make the terminal section bigger, hover over the top line of the terminal section with your mouse - it will change to an up-down arrow icon and then you can drag up which will also make the file editing area smaller.
 {% endhint %}

10. If we leave Cloud9 and come back to this workspace, the version of Node.js resets, so let's change the default. In the terminal, type: `nvm alias default 8`

11. Install the Angular CLI, type: `npm install -g @angular/cli`

 *This may take a minute or two to complete. Perfect excuse to grab yourself a drink!*

12.  To confirm Angular CLI was installed, type: `ng version`. If you get a version number, you can move on!

13. Continue with Part 1: Starting your Single Page App, Step 2.

 {% hint style='danger' %}
Keep your eyes out for Cloud9 sections that you need to expand and follow as you go through the worksheet. 

Any time the worksheet references Atom, iTerm2 or Git Bash, just know that your workspace is all inclusive and you'll just be working within Cloud9.
 {% endhint %}

<!--endsec-->
