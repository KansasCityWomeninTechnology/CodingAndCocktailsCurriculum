###Normalizing
We'll start with normalizing the styling.  This is necessary to help things look consistent across browsers (ie. Microsoft Edge, Google Chrome, Internet Explorer, Safari, etc.) as each browser implements features at different times or somtimes slightly different than how the others do.  

1. In the project pane on the left, right click on the sass folder and select `New File`. 

2. Type `_normalize.scss` and press enter. This will be the file where we set some styles that will set up more of a blank slate starting point for styling and set some basic styles.
    
2. Add the following to reset some default styles across browsers and allow a clean starting point for your styling.
    
    ```css
    /* Reset */
    html, body, div, h1, h2, h3, h4, h5, h6, p, a,
    img, li, aside, footer, nav, section {
            margin: 0;
            padding: 0;
            border: 0;
            font-size: 100%;
            font: inherit;
    }
    ```
    
3. In addition set the base styling for the body and headers. Add the following to your _ _normalize.scss_ file underneath the closing `}` for the reset styles.  Leave a blank line between the `}` and the following styles to improve readability. Make sure you replace the variables in the example below with the colors that you've chosen and set up as variables within your project.
    
    ```css
    body {
            background-color: $cream;
    }

    h1,h2,h3,h4,h5,h6 {
            color: $dark-green;
    }
    ```
    
4. The _ _normalize.scss_ file needs to be tied in to the project so in your _styles.scss_ file type in `@import “normalize”;` to import the _ _normalize.scss_ file.

6. Save both the _styles.scss_ and _ _normalize.scss_ files.

###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 
