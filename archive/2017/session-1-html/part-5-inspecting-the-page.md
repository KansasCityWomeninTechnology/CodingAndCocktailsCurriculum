#Part 5: Inspecting the Page
You'll often find yourself needing to look at how your page is being rendered in the browser to troubleshoot issues so let's give that a try.

1. In Google Chrome, right-click on your `h2` text and choose **Inspect**

    This will open up your Chrome Developer Tools to the **elements** tab
    
2. Notice you can see all of your tags that you've added to the page and how they are nested inside each other. It should look something like this:
![](/assets/devTools.png)

3. Notice as you mouse over elements in the Dev Tools that they are highlighted in the rendered view above.
![](/assets/highlight.png)

4. You can also click the arrows to the left of your `div` elements to expand them and see the elements inside them.

5. In addition, you can make and preview changes here before making them in your code.
    * In the **elements** section of the Dev Tools, double click on the text inside your `h2` tag. This should make it editable. Change it to "Hello World" and then press `enter` 
![](/assets/helloWorld1.png)

    * Your `h2` text should now display "Hello World" on your rendered page.
    ![](/assets/helloWorld2.png)
    
    {% hint style='danger' %}This only lasts until you refresh the page! If you want to make a lasting change you need to make the change to your code. {% endhint %}

    * Refresh your page to see your text return to what you have in your code.
    
6. You can either keep your Dev Tools open or close them with the small x in the upper right corner of the Dev Tools

    * Another quick way to open the tools at any time is through a keyboard short cut:
    
| Windows Key Combination|Mac Key Combination |
|---|---|
|`ctrl` + `shift` + `i`|`cmd` + `option` + `i`|

{% hint style='info' %}Element inspection comes in very handy when you're trying to style your page too so we'll use this a lot next month when we learn about CSS!{% endhint %}
