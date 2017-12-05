# Part 6: Images

Add an image to your about section to bring some interest to your page.

1. In Google Chrome, navigate to [flickr.com](http://flickr.com)

2. Search for a cocktail image

3. Change the license filter from "Any License" to "Commercial use allowed"

4. Choose your favorite image, click on it and click on the download icon in the lower right corner.  You get to choose what size you'd like on your page. You'll want to save it into your `CodingAndCocktails\html` folder.  Name it something easy to remember.

    ![](/assets/download.png)
    
5. In Atom, add an `img` tag just below the "About" header on your page.  
{% hint style='tip' %}Don't forget to use emmet to complete your tag for you - it will automatically add your `src` and `alt` attributes for you but you still have to fill out their content!  The `src` attribute tells your code where to look for your image and the `alt` attribute content gets displayed if your image is not able to be rendered and is used by screen readers for better accessibility. {% endhint %}

6. For your `src` attribute you'll need to point to where the file is.  Since we placed our image in the same folder we only need to provide the file name you chose in step 4 (including the file extension!) inside the quotation marks here.

6. Save your file and reload it in Google Chrome.

###Documentation

[Mozilla Developer Network image element documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img)




