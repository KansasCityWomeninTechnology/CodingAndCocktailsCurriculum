###Body Styling

{% hint style='danger' %}
If you're missing image files, navigate back to the [Sass Setup](/sass-setup.md) portion and run through steps 3.i through 3.v.
{% endhint %}


1. In the project pane on the left, right click on the sass folder and select `New File`. 

2. Type `_main.scss` and press enter. This will be the partial file where the styling for the main body portion of our page will be located.

3. Don't forget to import main into your _styles.scss_ file and save the file.

2.  Start with styling the main “hero” image and text with the large page heading, a smaller “tagline” and some about text.

    1. Select the `.hero` class.
    
    2. Give it a `height:` and a `width:`.  A `600px;` height should work well. It should cover `100%;` of the width of the page.
    
    3. Instead of having an `<img>` HTML element here to display the image, we'll be using a background image on our div.  
    
        1. Take a look at the [background property documentation on MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/background).  It is a pretty powerful property with the ability to set values for multiple background properties in one.  
        
        2. Set the `background:` property to `url("../images/hero.jpg") no-repeat center top;`.  
        
        {% hint style='info' %}
This is telling the background property that we are using a link to find our image (url = uniform resource locator).  Go up one directory/folder from where we are (`../`), look in the images folder (`images/`) and use the `hero.jpg` file as the background image.
        
Also we don't want to repeat the image, we just want a single image displayed (`no-repeat`).
        
The image should be `center`ed horizontally and align the `top` of the image with the top of the background layer.
        {% endhint %}
        
        3. Finally, make sure the `background-size:` is set to `cover;` to make the image cover the width and height of the container.
        
    4. Select the `.hero-text` class and give it a `width:` of `50%;` and add a `padding-top`.  See if you can find a good value for the top padding so it doesn't sit right at the top of the page and looks nice.
    
    5. Also make sure your text is centered.  Hint: https://developer.mozilla.org/en-US/docs/Web/CSS/text-align.
    
    6. Set the `color:` and `font-size:` to appropriate values for the `h1`, `h2` and `p` elements.
    
    7. You'll also want to add some extra margin on the bottom of the `h2` element to separate it from the `p` text.

3. Below the "hero" set up two columns for your main page content and a sidebar.  We'll use the flexbox model here to help us out.

    For more information on using flexible boxes see https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes.
  
  1. Select the `.flexbox` class.
  
  2. Add the `display:` property with the `flex;` value to set up our layout.
  
  3. We're setting up just a single row with this so set the `flex-flow:` property to `row;`.
  
  3. Nested inside the flexbox selector, add a selector for the `.col-1` class.
  
  4. To set the size of `.col-1` set the `flex:` property to `3 1 75%;`.  This will tell the first column how much space to take up inside the `.flexbox` flex container.
  
  5. After the `}` for the `.col-1` rules, add a selector for `.col-2`.  Set the `flex:` property to `1 3 25%;` 
  
  6. In the `.col-2` styles you'll also want to change the `background-color:` and `font-size:`.

4. Style the menu item list.

    1. Select the drinks class.
    
    2. Remove the bullets from the list. (Remember how you did this in the nav styling?)
    
    3. Nested in the drinks selector, select the `h2` element and set a `font-size` and `margin` of `3em` and `5px` respectively.
    
    4. Nested in the drinks selector but after the closing `}` of the h2 selector, select the `item` class.  The ellipses `...` indicate code not written out in the example, they should not be a part of your code.
    
    ```sass
    .drinks {
            ...
        
            h2 {
                ...
            }
        
            .item {
            }
    }
    ```
    
    5. Add a `margin-bottom:` of `60px;`
    
    6. Add a top 1 pixel dotted border that is one of the colors from your color palette
    
    7. Set the top padding to `10px;`
    
    8. Set the `display:` property to `block;`
    
    9. Nested in the drinks selector but after the closing `}` of the item class selector, select the `head` class.
    
    10. Enlarge the head font size to twice that of the current font size.
    
    {% hint style='tip' %}
1em is equal to the current font-size of the element in question
    {% endhint %}
    
    11. Nested in the drinks selector but after the closing `}` of the head class selector, select the `p` (paragraph) element.
    
    12. Enlarge the paragraph font size to 1.3 times the current font size.
    
    13. Nested in the drinks selector but after the closing `}` of the `p` element selector, select the `img` (image) element.
    
    14. `float:` the image `left;`.
    
    15. Add a margin, height and width for your image.  Suggested values are:
    
    ```css
    margin: 0 20px;
    height: 120px;
    width: 120px;
    ```
    
    16. Save your file.
    
    17. In the command line, type `sass --watch sass/styles.scss:css/styles.css` so sass will watch for changes to your scss file and automatically compile them.  
    
    {% hint style='tip' %}
Use the key combination `ctrl` + `c` to get back to your command prompt.
    {% endhint %}
    
    18. Use a `border-radius:` to make the image circular.  Try different values to see what they look like.  Save the file and refresh in Google Chrome to view changes.  
    
    {% hint style='tip' %}
Since sass is set to watch for changes we are taking out the manual step to compile the Sass into CSS.
    {% endhint %}
    
    19. Nested in the drinks selector but after the closing `}` of the `img` element selector, select the `a` (anchor) element. 
    
    20. Remove the text decoration and set the text color. Hint: https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration
    
    21. Check out your page content in Google Chrome.  Things should be looking like they're coming together now!
    
7.  Style the sidebar "Small Plates" content on the right side.

    1. Below the closing `}` for the drinks class selector, select the sidebar class.
    
    2. See if you can style the `h2` and `ul` elements inside the sidebar class to look similar to the example image that you can view here: https://raw.githubusercontent.com/KansasCityWomeninTechnology/CSSCompilerPractice/master/ladyDevBarAndGrill.png 
    
8. Save the _ _main.scss_ file and reload the page in Google Chrome.  Your page should be looking a _lot_ more stylish than when we started! Keep up the hard work!

###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 
