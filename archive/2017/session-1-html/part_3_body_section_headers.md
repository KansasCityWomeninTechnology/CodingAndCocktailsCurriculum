# Part 3: Headers & Page Sections

The body section of your HTML contains the visible part of your webpage.  Let's start building out some content!

1. We'll create sections within our page with `div` tags.  

    1. In Atom, between the opening and closing `<body></body>` tags, type `div.container` and press the `tab` key.  This will create a `div` element with a class attribute with the value of container and will be the main container element for our page.
    
    {% hint style='tip' %}
    Anytime you want to add a `class` attribute to an element you can add that by adding a period and then the classname you want to add when you're using emmet to create your elements. {% endhint %}

    {% hint style='tip' %}
    An `id` attribute can be added by typing a `#` and then the name of the id you'd like to set.
    {% endhint %}
    
    {% hint style='info' %}
    Want to know the difference between an id and a class?  Check out http://bit.ly/CnCIDvsClass
    {% endhint %}
    
    Your body section should now look like this: 
    ```html
    <body>
            <div class="container"></div>
    </body>
    ```

    2. Nested inside the `div.container` create another `div` element with the class `row`. Type `div.row` and press the `tab` key. _Don't forget to indent so your code is easy to read!_
    Your body section should now look like this: 
    ```html
    <body>
            <div class="container">
                <div class="row"></div>
            </div>
    </body>
    ```
    
    {% hint style='info' %}
    Classes are often used to apply styling to elements - we will learn about styling next month. We'll see this in action later in the worksheet.  For now, don't worry too much about what the classes mean - we're focusing on the HTML this month.
    {% endhint %}
    
    4. Save the page, switch over to Google Chrome and reload.  Even though we've started adding content to the `body` section there is still nothing to see.
    
    {% hint style='tip' %}
    If the file has not been saved you'll notice a small blue dot on the right side of the file's tab.  That goes away when the file has been saved.  The active tab has a blue line to the left so in the image below index.html is the selected tab and changes have not been saved.
    {% endhint %}

    ![](/assets/atom.png)

2. Create an `h1` tag inside the last `div` element. Type `h1` then press the `tab` key. Write the name of your cocktail lounge between the opening and closing tags.

4. Save your file and reload it in Google Chrome. **We have content!**

    ![](https://media.giphy.com/media/3o6gEeg80PqeJBtsdy/giphy.gif)
                        
4. After the closing `h1` tag, add an `h2` tag for a subtitle containing the text "Cocktails with a side of code." 
    It should look something like this: 
    ```html
    <body>
        <div class="container">
            <div class="row">
                <h1>Coding's Cocktail Lounge</h1>
                <h2>Cocktails with a side of code</h2>
            </div>
        </div>
    </body>
    ```

5. Next, we'll want an "About" section, a "Menu" section, and a "Contact" section using more `div` tags. We'll need to add `id` attributes to these `divs` for navigation later in the worksheet.
    
    1. Inside the `div.container` element but below closing `</div>` tag for the first `div.row` element, type `div.row#about` and press the `tab` key.  This will be the area for our "About" section. The element you created should look like this:
    ```html
    <div class="row" id="about"></div>
    ```
    
    {% hint style='tip' %}If you place your cursor on any HTML element, Atom will underline the matching opening or closing tag for you. {% endhint %}
    
    3. Inside that about `div`, we'll title the section.  Since this is the third most important heading on the page we'll use an `h3` tag. Place the text "**About**" between the tags.
    
6. Repeat this process twice more for the Menu and Contact sections.

    1. In between the opening and closing tags for the `div.container` element but below the closing `</div>` tag for the about section, type `div.row#menu` and press the `tab` key. This will be the area for our "**Menu**" section.

    3. Inside the menu `div`, title the section with the text "**Menu**" using an `h3` tag.
    
    4. In between the opening and closing tags for the `div.container`, below the menu section, add a row with the id of "contact."  row. 

    6. Create an `h3` tag with the text "**Contact**" between the opening and closing div tags created in the last step.

7. Save your file and reload it in Google Chrome. Your page should look similar to this:
![](/assets/headersSectionsEnd.png)

###Documentation

If you want to read up on header or div elements check out the documentation from Mozilla Developer Network:

[MDN Documentation on heading elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements)

[MDN Documentation on div elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/div)