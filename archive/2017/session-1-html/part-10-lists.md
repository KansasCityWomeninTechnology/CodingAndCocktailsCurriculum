#Part 10: Lists

Lists often come in handy on a webpage - both ordered (numbered) lists and unordered (bulleted) lists.  Website navigation is often an unordered list of links so that's where we'll be using a list. We have three page sections - About, Menu, and Contact - so we'll need three navigation list items.

 1. In Atom, use the magic of emmet to make your life easier.  In between the opening and closing `nav` tags, type `ul.nav.navbar-nav>li*3` and push the `tab` key.  Voila! An unordered list with two classes and three list items ready to go!
 {% hint style='info' %}You told emmet that you wanted an unordered list (`ul`) with a `.nav` class and a `.navbar-nav` class with child (`>`) list item elements (`li`), three of them (`*3`) {% endhint %}
 
 2. In between each list item's opening and closing tags type the section names **About**, **Menu** and **Contact**.
 
 3. Save your file and reload it in Google Chrome.
 
Navigation items display on the page but don't yet navigate anywhere - add that in Part 11.

###Documentation

[Mozilla Developer Network unordered list element documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)

[Mozilla Developer Network list item element documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/li)

[Mozilla Developer Network ordered list element documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)