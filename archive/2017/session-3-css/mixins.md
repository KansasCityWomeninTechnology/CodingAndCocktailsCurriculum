##Mixins

Let’s try a mixin now! We can use one for list styling, let’s call it `list-reset`.

1. In the project pane on the left, right click on the sass folder and select `New File`. 

2. Type `_mixins.scss` and press enter. This will be the partial file where any mixins we us in our project will be located.

3. Don't forget to import mixins into your _styles.scss_ file.  Since we'll be using some of these mixins in the _ _nav.scss_ and _ _footer.scss_ files it will need to be imported before those files are imported.

4. Add your mixin to the _ _mixins.scss_ file. This is adding a “function” to set the three properties `list-style`, `margin` and `padding` anytime this mixin is used in your Sass file:

    ```sass
    @mixin list-reset() {
        list-style-type: none;
        padding: 0;
        margin: 0;
    }
    ```

5. In your _ _nav.scss_ and _ _footer.scss_ files, replace the `list-style-type: none;` code with `@include list-reset();`

4. Save your _ _nav.scss_, _ _footer.scss_, _styles.scss_ and _ _mixins.scss. files.

5. In the command line type `sass sass/styles.scss css/styles.css`.

6. Go to Google Chrome and refresh your page. It should look the same but now you're consistently setting list styles across the project and have a single place to go change them should you need to in the future.

###Documentation
To understand the different CSS properties and available values visit the [Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

View the Sass documentation here if you want more detailed information about how any pieces of Sass work: [bit.ly/CnCSassDoc](http://bit.ly/CnCSassDoc) 