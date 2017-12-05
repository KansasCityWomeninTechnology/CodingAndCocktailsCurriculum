# Part 8: Forms

Under the "Contact" header add a form to allow users to contact you. Forms typically require a bit of JavaScript but that tool is not in our toolbelt just yet we'll use a tool called Formspree. You can read up on it at [formspree.io](https://formspree.io/).

1. In Atom, under the "Contact" header add a `<form></form>` element to your page.

2. Set the `action` attribute's value to `https://formspree.io/youremail@example.com` replacing the `youremail@example.com` text with your actual email address.

3. Add a `method` attribute to your `form` element with a value of **"POST"**. This is required to make the form work with Formspree.
{% hint style='tip' %}Remember attribute values are surrounded by double quotation marks! {% endhint %}

4. The form will have sections for a name, an email address and a message along with a **Submit** button.
    
    1. Inside the `form` element type `div.form-group*4` and push the `tab` key to add the four form sections.
    {% hint style='info' %}You asked emmet to create a div element (`div`) with the class form-group (`.form-group`), four of them (`*4`){% endhint %}
    
5. The first section is the name section. In between the first opening and closing `div.form-group` tags, add a `label` element. Type `label`  and push the `tab` key
    
     2. Set the label's `for` attribute value to **"nameInput"**
     
     3. Add the text **"Name"** in between the opening and closing label tags.
    
     3. Just below the label element type `input#nameInput.form-control` then press the `tab` key to create your input element with the id **"nameInput"** and class **form-control**.
     {% hint style='info' %}Remember, ids are created by using a `#` followed by the id name you want to add and classes are created by using a `.` followed by the class name you want to add{% endhint %}

     4. Add a `name` attribute to that `input` element and set it's value to **"name"**

     {% hint style='tip' %}Emmet will automatically add your `type` attribute and leaving it with the value "text" for our first input is perfect!{% endhint %}
     
     5. Also add a `placeholder` attribute and set the value to **"First and Last Name"**. 
     Your code should look similar to this now:
     ```html
     <div class="form-group">
         <label for="nameInput">Name</label>
         <input type="text" id="nameInput" name="name" class="form-control" placeholder="First and Last Name">
     </div>
     ```   
    
6. Save your file and reload it in Google Chrome.  The form is starting to come together!  It should look like this:
    
    ![](/assets/firstForm.png)
    
7. The second section will be for the user email address. In between the opening and closing tags for the second form-group div, add a `label` element. 

    1. Set the `for` attribute to **"emailInput"** 

    2. In between the opening and closing tags set the text to **"Email Address"**.
    
    3. Below the `label` element, add an `input` element with an id of **"emailInput"** but this time set the `type` attribute to **"email"**
    
    4. On the `input` element, add a `name` attribute with a value of **"_replyto"**.  This is another requirement to make the form work with Formspree.
    
    5. Add a `class` attribute of **"form-control"**.
    
    6. Add a `placeholder` attribute with a value of **"Email Address"**
    
8. Save your file and reload it in Google Chrome. Progress! It should look like this:

    ![](/assets/secondForm.png)
    
9. Create the area for the message. Inside the third form-group add a `label` element.

    1. Set the `label` element's `for` attribute to **"messageInput"** 
    
    2. Add text **"Message"** in between the opening and closing `label` tags.
    
    3.   Below the label, add a `textarea` element with a `class` of **"form-control"**.
    
    4. Set the `name` attribute of the `textarea` element to **"message"**
    
    5. Set the `id` attribute to **"messageInput"** 

    6. Leave the `cols` and `rows` attributes at the default values provided.
    
    7. Add a `placeholder` attribute with a value of **"Message Text"**.
    
    {% hint style='info' %}Why are we using a textarea element instead of an input element here?
    Look at the MDN documentation for input linked at the bottom of the page. Scroll down to the `type` attribute and look at the explanation for the value of "text".  This shows it only allows a single line of text to be entered when the input elements `type` attribute is set to "text".  Since a message is usually multiple lines, a `textarea` element is a better choice for the message.{% endhint %}
    
10. Save your file and reload it in Google Chrome. It should look like this: 
    
    ![](/assets/thirdForm.png)
    
11. In between the the final form-group `div` opening and closing tags, add an `input` element with a `type` value of **"submit"**.

     1. Add two classes: **btn** and **btn-default**.
     
     2. Add a `value` attribute with a value of "Send". 
    
    {% hint style='tip' %}Type `input.btn.btn-default` and then press the`tab` key to add both classes to the input element at the same time{% endhint %}
    
    {% hint style='info' %}The `value` attribute sets the text of the submit button so feel free to set the text to whatever you'd like!{% endhint %}

12. Save your file and reload it in Google Chrome. The final form should look like this: 
    
    ![](/assets/fourthForm.png)    
 
{% hint style='info' %}Since our websites are not deployed to a server, the form won't actually work right now. 

If you'd like to try putting your site up on the internet ask a mentor to help you push it up to GitHub Pages and then you can test out your form.  The way Formspree works is that you'll have to test it once, which will send you an email asking you to confirm your email address and from then on, your form will be functioning!{% endhint %}

###Documentation

[Mozilla Developer Network form element documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form)

[Mozilla Developer Network input element documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input)

[Mozilla Developer Network textarea element documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/textarea)