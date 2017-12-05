###Nav Styling
Style a horizontal navigation bar.

Check out w3schools navigation styling if you'd like some additional examples or an alternate explanation: [bit.ly/NavCSS](http://bit.ly/NavCSS)

1. In the project pane on the left, right click on the sass folder and select `New File`. 

2. Type `_nav.scss` and press enter. This will be the partial file where the styling for the navigation bar in our project will be located.

3. Don't forget to import it into your _styles.scss_ file.

3. The navigation menu is a list of links. Start by selecting the `nav` element in the _ _nav.scss_ file.

4. Set up some basic styling for the `nav` by setting the following properties:

    * `background-color:`
    
    * `text-align:` 
    If you'd like to align your items to the right like in our sample image set this to `right;`.
    
    * `font-family:`
    
    * `border-bottom:` 
    You might choose to lighten or darken your background-color here by using `lighten($my-color, 20%)` to lighten it by 20% or `darken($my-color, 20%)` to darken it by 20%. A solid border would be most appropriate here.

3. The bullets on the list don't make for a visually appealing.  Since the `ul` (unordered list) element is a child of the `nav` element, nest the `ul` selector inside the `nav` element selector.  It should look something like this where the `...` ellipsis indicate code not shown in the example:

    ```sass
    nav {
        ...
        ul {
        }
    }
    ```

4. Remove the bullets from the `ul` by using the `list-style-type:` property and setting it to the value `none;`.  Your styling should now look something like this:

    ```sass
    nav {
        background-color: $orange;
        text-align: right;
        font-family: $body-font;
        border-bottom: 5px solid lighten($orange, 20%);
        
        ul {
            list-style-type: none;
        }
    }
    ```
    
4. Also nested inside the `nav` selector, select the `li` (list item) elements.  Make sure these have styling of `display: inline;` to make sure they are shown in a horizontal row and `padding: 2px;` to space the items out a bit.

5. Finally, style the `a` (anchor) elements. Set the following properties on these:

    * Set `display:` to `inline-block;` to make sure everything stays on the same horizontal line.
    
    * Set `padding:` to `6px 20px;` to give some space around the text.  This will put a 6 pixel padding on the left and the right and a 20 pixel padding on the top and bottom.  
    
    * Set `text-decoration:` to `none;` to remove the underline on the link text.
    
    * Set `font-weight:` to `bold;` to make the text a bit heavier.
    
    * Set the font `color:` to one of your chosen color palette's color variables `$white;`
    
    * Set the `font-size:` to `1.5em;` to make it a bit larger and easier to read the page navigation.
    
5. Save the _styles.scss_, and _ _nav.scss_ files.

6. Now compile the Sass into CSS. 
    
    1. In the command line (Git Bash for windows, iTerm2 for macs) make sure you are in the folder containing your _index.html_ file.
    
    2.  Type: `sass sass/styles.scss css/styles.css`

8. Go to Google Chrome and refresh your page. You should have a more visually appealing navigation bar now.

    
###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 