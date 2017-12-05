###Variables
Start by creating some Sass variables that will represent the colors in the color palette that you selected earlier.

1. In the project pane on the left, right click on the sass folder and select `New File`. 

2. Type `_variables.scss` and press enter. This will be the file where all of our variables that we use in our project will be located.
    
3. Open that file if necessary and in that file create your first variable for the main color of your site. Variables start with a `$` followed by the variable name.  It might look something like the following:
    
    ```
    $orange: #cb6f10;
    ```
    
4. Create variables for the remaining colors in your site.  It is common to name your color variables according the color name.  Things like `$turquoise`, `$white`, `$dark-purple`, etc.

5. The variables file needs to be tied in to the project so in your _styles.scss_ file type in `@import “variables”;` to import the _ _variables.scss_ file.

6. Save both the _styles.scss_ and _ _variables.scss_ files.

###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 