# Part 3: Variables & Aliases

---

#### Creating variables and aliases

Variables can be created with the `export` command. Several programs and utilities use built in variables programmatically. Here's how to create and also how to display variable values:

1. Type `export MY_FAV_DRINK=Greyhound` ![](images/enter.png). Feel free to put in any value you'd like!
    {% hint style='info' %}
Be careful when including spaces - in that case, you'll want to enclose your value in quotation marks so it doesn't break up the command, i.e. `export MY_FAV_DRINK="Horsefeather"`.
    {% endhint %}

2. Type `echo $MY_FAV_DRINK` ![](images/enter.png) in your command line.
    {% hint style='tip' %}
Note the `$` at the beginning of the variable.
    {% endhint %}

  Now try displaying the values for the built-in OS variables of HOME and USERNAME. Remember, you should use the syntax `echo $VAR`.

#### The PATH variable

  **PATH** is a unique variable. It includes the locations of all executables, which are files or programs able to be run by a computer. When you run a command, your shell looks in the directories specified there for an executable with a matching name. Most installers modify your path automatically for you to include any new paths needed! Let's check out what's included in our path:

1. Type out `echo $PATH` ![](images/enter.png).
    {% hint style='info' %}
To add directories to the PATH, you would use the syntax `export PATH=/some/directory:$PATH`. Notice that you can reference the PATH variable in creating the new PATH.
    {% endhint %}
    {% hint style='danger' %}
Be **VERY** careful editing your PATH as you could loose access to your programs!
    {% endhint %}

  So what's an alias? Basically, it's a shortcut you create to a command. For example, remember the `ls -al` command we used earlier? You can add an `-h` option to show file sizes in a more **h**uman readeable format. The command `ls -alh` gives us more information and makes the output easier to read. Let's bind it to a new command, `la`, to save us some keystrokes:

2. Enter `alias la="ls -alh"` ![](images/enter.png).

  Now you can type `la` ![](images/enter.png) and get the output for `ls -alh` instead. You can imagine how much time this customization can save!
    {% hint style='tip' %}
The command `ll` is a built-in alias for `ls -al`.
    {% endhint %}

#### Making aliases and variables persistent

  Now, close out of your terminal and open a new one. You'll notice that the alias we just create didn't persist. That's because every time you open a new terminal, its settings, namely what's called your **profile,** are reloaded.

You can edit your profile by following these steps:

1. Create the file by typing `touch ~/.bash_profile` ![](images/enter.png).
    {% hint style='info' %}
If the file already exists, its timestamp will be updated but no harm will be done.
    {% endhint %}

2. Type `vim ~/.bash_profile` ![](images/enter.png). Then add the alias command we used above using INSERT mode with `i`.
    {% hint style='tip' %}
Jump back to [**Part 1**](/part-1-navigation-and-basics.md) if you need some help with navigating in vim.
    {% endhint %}
    {% hint style='info' %}
Your custom variables, like the $MY_FAV_DRINK we set above, will also be lost when you close your terminal. You can add custom variables to your ~/.bash_profile as well by adding the `export MY_FAV_DRINK=Greyhound` command, for example, in its own line.
    {% endhint %}

3. Type`source ~/.bash_profile` ![](images/enter.png) in your command line. This will load or reload your profile settings.
