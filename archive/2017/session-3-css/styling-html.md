#Styling HTML

1. In CodePen, notice we've set up some HTML for you to practice styling.  There is already page structure content in the first box with the HTML heading.

2. In the middle box with the CSS heading, select the `body` element and change the `background-color` property to the hexadecimal color from your selected color palette.

    {% hint style='tip' %}
Remember the syntax for a CSS rule looks like this:
```css
selector {
      property: value;
}
```
    {% endhint %}

3. Select the `ul` element and set the `list-style-type` to `none`. Notice how the bullets disappear from each of the list item elements.

4. Since the list items (`li` elements) are being used for navigation purposes here, change them to have `display: inline;` styling.  Notice how that makes them sit next to each other instead of on top of each other.

5. Select the element with the id `#main-title`.
    
    1. Change the `font-family` to the font name that you selected from google fonts.
    
    2. Increase the size of the text to be four times the size of the HTML (root) font-size. 
    
    {% hint style='tip' %}
1rem is equivalent to the HTML (root) font-size.
    {% endhint %}
    
    3. Change the `color` to another color hex value from your chosen color palette.

    4. Center the header text using the `text-align` property.

6. Select the `img` element.

    1. Change the height of the image to `100px`.
    
    2. Change the width of the image to `200px`.
    
    {% hint style='danger' %}
Notice how this distorts the image so when you are styling an     image make sure to keep an eye to how your styling affects the     image.
    {% endhint %}

7. Select the `.section` class and change the `background-color` to another color within your chosen palette.

    Notice how the div sections don't stretch to meet the edges of the page body or eachother
    
8. Select the first section with the `.section-one` class
    
    1. Add a `border` that is 5 pixels wide and solid using another of the colors from your chosen palette.
    
    2. Add a `margin` of `20px`. Notice how that made your border box move and added space around the _outside_ of your border.
    
    3. Add some `padding` of `40px`. Notice how that made the border box bigger around the text content and added space _inside_ your border.
    
9. In the view section scroll down until the link comes into view.  
    
    1. select the `a` (anchor) element and use the `text-decoration` property to remove the underline.

    
###Documentation
[Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)