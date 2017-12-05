# Part 11: Anchors (aka Links)

The navigation items should take the user to the page sections they reference. In order to do that, anchor elements need to be added to create a hyperlink to those sections of the page.

1. In Atom, select the **"About"** text in the first list item and use the keyboard shortcut below to wrap a tag around other content.

Windows Key Combination|Mac Key Combination
---|---
`ctrl` + `alt` + `w`|`ctrl` + `w`
    
2. Type just an `a` in the prompt that comes up and press enter. An anchor tag with an `href` attribute will show up wrapped around your **"About"** text. The **"About"** text should now look like this: 
    ```html
    <li><a href="">About</a></li>
    ```

3. The href attribute tells the anchor where to go when it is clicked.  Clicking **"About"** should move to the **"About"** section of the page.  The about section is the `div` element with the id `about`.  Set the anchor tag's `href` value to **"#about"**.

4. Repeat this process for the Menu and Contact sections.  

5. Save your file and reload it in Google Chrome.

We now have a working navigation section!
{% hint style='tip' %}Since we don't have a lot of content on our page it may not appear to work at first.  If you shrink the size of your browser window down so it is about half as tall, try clicking on the menu navigation item again and the menu section should show at the top!{% endhint %}

###Documentation

[Mozilla Developer Network anchor element documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a)











