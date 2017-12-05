# Part 9: Navigation & Footer

Most websites have a way to navigate around.  HTML 5 added `nav` and `footer` elements to the mix so let's practice using those!

1. In Atom, create a navigation row section and add the navbar.
    
    1. Above the first `div.row` (now displayed in your code as a div element with the row class - `<div class="row"></div>`) add a new `div.row`.
    
    ![](/assets/navInsert.png)
    
    3. In between the opening and closing `div` tags just created, add a `nav` element with the classes **navbar** and **navbar-default** inside the div from step ii.
    
    4. Save your file and reload it in Google Chrome.
    {% hint style='info' %}Nothing to see here. How does a user move around? We'll add the navigation links in Part 11: Anchors!{% endhint %}
    
2. Create a footer row section and add a footer.  

    1. Add another `div.row` just inside the `</div>` tag that is closing the `<div class="container">` element.
    
    3. Add a `footer` element in between the opening and closing tags of that `div.row`.

    4. Footers often contain copyright information so try using an [HTML entity](http://www.w3schools.com/html/html_entities.asp) to add a copyright symbol. In between the opening and closing `<footer></footer>` tags add the text `&copy;` and the text " Copyright your name 2017"

3. Save your file and reload it in Google Chrome.

###Documentation

[Mozilla Developer Network nav element documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav)

[Mozilla Developer Network footer element documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer)



