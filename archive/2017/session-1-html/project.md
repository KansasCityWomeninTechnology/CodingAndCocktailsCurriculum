# Project

HTML provides your website with the underlying structure.  We'll start with a basic HTML structure and continue with adding page content.

{% hint style='danger' %}
If you are using a Chromebook, please skip to the Chromebook Only section below!
{% endhint %}

## Part 1: HTML Page Structure
We'll explore using the Emmet plugin in the Atom text editor that we use as our development environment.  This plugin helps us write our code faster and more efficiently.

1. In the CodingAndCocktails folder you created during the tools setup create a folder called `html`.
2. Open Atom.
3. Go to the `File` menu and choose `Add project folder`.
4. Navigate to and select the `CodingAndCocktails\html` folder.
3. On the left side of your screen, right click on the `html` folder and select `New file`.
5. Name the file _index.html_ and press enter to save it in your `CodingAndCocktails\html` folder.
6. In the project pane on the left, double click on the _index.html_ file to open it.
7. In your _index.html_ file type `html:5` and press the `tab` button on your keyboard.  This is some of the magic emmet can help us with and should come out looking like the following: 

  ```html
  <!DOCTYPE html>
  <html lang="en">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>Document</title>
  </head>
  <body>
  
  </body>
  </html>
  ```
See how the `meta` and `title` tags are indented since they are children of the `head` tag?
{% hint style='danger' %}Setting up the HTML structure with emmet this way only works when the file you're developing in is already saved with the .html file extension. {% endhint %}
6. Cheers! You just set up the structural foundation of a web page!

<!--sec data-title="Chromebooks Only: Cloud9 Instructions" data-id="section0" data-show=true data-collapse=true ces-->

1. Sign up for an account at [c9.io](https://c9.io)
   
   Note: It will ask you for credit card information but you will not get charged for anything since we do not use features of Cloud9 that cost money.

2. Confirm your account from your email and log in to Cloud9.

3. Select `Workspaces` from the left side panel if you are not already there.

4. Choose `Create a new workspace`.

5. Pick a name for your workspace and enter it - it can be anything you'd like.  You do not need a description but feel free to add one if you'd like.

6. Leave your workspace as a "Public workspace".

7. In the template section choose `HTML5`

8. Click on the `Create Workspace` button

   Cloud9 will take a minute and create your workspace here
   
9. Close the README.md file that is open when you get to your workspace.

10. From the `File` menu choose `New File`

11. From the `File` menu choose `Save As...` and use the file name _index.html_.  It should default to the workspace folder and display `/` in the `Folder` text box at the bottom, leave that as-is.

12.  Click the green `Save` button

13. In the top menu bar choose `Preview` and then select `Live Preview File (index.html)`

    This opens up a "browser" window that will show changes you make to your web page as you add content.  
    
    {% hint style='danger' %}
    IMPORTANT! Any time the worksheet references viewing in Google     Chrome or refreshing the page in Google Chrome you will use this Preview area instead.
    {% endhint %}

14. Continue with step 8 above. Luckily Cloud9 also lets us use the magic of emmet.

    {% hint style='danger' %}
    Cloud9's initial page structure will be missing two of the above mentioned meta tags.  This is okay - you can ignore it and continue on with the worksheet.
    {% endhint %}
<!--endsec-->

