##Footer Styling
Style a footer with copyright information and social media links.

1. In the project pane on the left, right click on the sass folder and select `New File`. 

2. Type `_footer.scss` and press enter. This will be the partial file where the styling for the main body portion of our page will be located.

3. Don't forget to import footer into your _styles.scss_ file.

4. See if you can set some styles for the footer on your own.  The example image can be found here: https://raw.githubusercontent.com/KansasCityWomeninTechnology/CSSCompilerPractice/master/ladyDevBarAndGrill.png

    You might be able to look at the _ _nav.scss_ file for some styling ideas. Also be sure to look at the Mozilla Developer Network (MDN) documentation linked at the bottom of the page to read about the CSS properties you want to use. If you get stuck call a mentor over to talk it through!

    {% hint style='tip' %}
Notice in the MDN documentation that you can open the examples and play with them in CodePen.  JSFiddle is another similar tool but since we used CodePen earlier you should already have an account there.
    {% endhint %}
    
    ![](/images/mdn-doc-codepen.png)
    
6. Save your _styles.scss_ and _ _footer.scss_ files and compile the Sass into CSS. 
    
    1. In the command line (Git Bash for windows, iTerm2 for macs) make sure you are in the folder containing your _index.html_ file.
    
    2.  Type: `sass sass/styles.scss css/styles.css`

7. Go to Google Chrome and refresh your page. You should have a more visually appealing footer now.  If it doesn't look quite like the sample image try setting some more styles and see if you can get it closer.  Don't forget to save, compile and refresh your page in Google Chrome to see your changes!


###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 
