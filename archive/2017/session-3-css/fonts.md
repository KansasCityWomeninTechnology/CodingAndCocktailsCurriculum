###Fonts
Add fonts for your page.

1. Back in Google Fonts ([fonts.google.com](https://fonts.google.com/)), make sure you have at least two fonts selected, one to use for headers and one to use for body text.

2. This time we'll find the `import` way of embedding the fonts by clicking on the red @IMPORT header next to the STANDARD header.

    ![](/images/font-import.png)

3. Copy the just the import statement for your fonts, not the surrounding `<style></style>` tags and paste it as the first line in your _styles.scss_ file.

4. In the _ _variables.scss_ file, set up the variables for `$body-font` and `$header-font` referencing the Google Fonts font-families. Depending on what fonts you've chosen, one variable might look like: `$body-font: "Work Sans", Arial, Helvetica, sans-serif;`

    {% hint style='tip' %}
If you select a font that has a name that is two words you'll need to wrap the font name in quotation marks.
    
Often you'll want to provide backup fonts for the page to fall back on in case it can't load the chosen font. A common fallback for sans-serif fonts might include Arial, Helvetica, sans-serif. For serif fonts it might include "Times New Roman", Times, serif as backups.
    {% endhint %}

5. In the _ _normailze.scss_ file, add the `font-family:` property to both the `body` selector and the `h1, h2, h3, h4, h5, h6` selector.  Set the values to the `$body-font;` and `$header-font;` respectively.

5. Save the _ _variables.scss_, _ _styles.scss_, and _ _normalize.scss_ files.

6. Now compile the Sass into CSS. 
    
    1. In the command line (Git Bash for windows, iTerm2 for macs) make sure you are in the folder containing your _index.html_ file.  Cloud9 users will already be in the right folder.
    
    {% hint style='tip' %}
The command `cd` will let you change directory (or folder).
The command `ls` will list the files in your current directory.
The command `pwd` will print working directory, or, show you what directory (or folder) you're currently in.
    
Join us in March for more information on these commands and more as we learn about the Command Line!
    {% endhint %}
    
    2.  Type: `sass sass/styles.scss css/styles.css`

7. Go to Google Chrome and refresh your page. You should notice the font styling has changed.

###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 