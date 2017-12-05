# Part 4: Pipes & Redirects

---

#### Passing output to stream

**Pipe** is used to pass output to another **program or utility**. **Redirect** is used to pass output to either a **file or stream**.

A stream is input/output of data travelling between processes which can be standard input \(stdin\), standard output \(stdout\), and standard error \(stderr\). Let's start by looking at an example of redirecting to a stream.

1. Type `sort << END` ![](images/enter.png). You'll be taken to a new line with a `>` prompt.
    {% hint style='info' %}
The **END** can actually be any word you want. You're telling `sort` to accept input until a specific value is given.
    {% endhint %}

2. Type in a cocktail name and hit enter. Enter in as many cocktails as you can think of, each on its own line.

3. When you're done, type `END` ![](images/enter.png).

    The sorted list of your cocktails now shows as your output.

#### Redirecting output to a file

You can also redirect to a file. Let's a make a list of our favorite beverages.

1. Create a new variable by typing `export MY_FAV_COLOR=purple` ![](images/enter.png). Feel free to change `purple` to whatever you'd like.

{% hint style='tip' %}
To keep everything organized, make sure you're in your CommandLineBasics directory before running this next command! Use the `cd` command to navigate there!
    {% endhint %}

2. Enter `echo "My favorite color is " $MY_FAV_COLOR > fav_color.txt` ![](images/enter.png), then `cat fav_color.txt` ![](images/enter.png) to see the results.

3. Let's add our second favorite color. Type `echo "My second favorite color is green" > fav_color.txt` ![](images/enter.png), then `cat fav_color.txt` ![](images/enter.png).

    Hmm, what happened there? Oh, we'll actually need to use the redirect to **append** instead! The `>` we used prior will overwrite whatever was previously in the file. We can use `>>` instead to append instead of overwrite.

    Let's try that again.

4. Enter `echo "My favorite color is " $MY_FAV_COLOR > fav_color.txt` ![](images/enter.png), then `cat fav_color.txt` ![](images/enter.png).
    {% hint style='tip' %}
Remember you can use your up arrow here to scroll through your prior commands!
    {% endhint %}

5. To add your second favorite color type `echo "My second favorite color is green" >> fav_color.txt` ![](images/enter.png) then `cat fav_color.txt` ![](images/enter.png).

#### Pipes

A pipe is a chain of processes so that output of one process \(stdout\) is fed to the input \(stdin\) of another.

Another command,`less`, allows you to "scroll" through output. We'll use the `history` command and pipe `less` to it in the examples below. The `history` command is very useful if you need to search through your previous commands.

1. In your command line, type`history > history.log` ![](images/enter.png).
2. Now enter `cat history.log | less` ![](images/enter.png).
    {% hint style='info' %}
You'll see '**:**' at the bottom of the terminal. Hit Enter or your up/down arrows to continue scrolling. Hit 'q' to quit.
    {% endhint %}

    You can also chain redirects and pipes. Here are a couple of examples to try:

3. Enter `sort -r < history.log > history_sorted.txt` ![](images/enter.png), then type `cat history_sorted.txt | less` ![](images/enter.png) to scroll through your sorted list.
    {% hint style='info' %}
The `sort` command is just what it sounds like. The command `history` outputs oldest command to latest command at the bottom, but you're probably more interested in your more recent commands, so let's reverse the order. The `-r` is there so we can reverse the order of the sort.
    {% endhint %}

4. Type `history | sort -r > history_pipesorted.txt` ![](images/enter.png), then type `cat history_pipesorted.txt | less` ![](images/enter.png) again.
    {% hint style='info' %}
This command is another way of getting the same output as the prior command. The only difference is that the commands we've ran since our last `history` commands will now be included.
    {% endhint %}

5. Enter `history | grep cat | sort -r > history_grep.txt` ![](images/enter.png), then `cat history_grep.txt` ![](images/enter.png).
    {% hint style='info' %}
The `grep` command searches text for the occurence of a specified string, in this case `cat`.
    {% endhint %}
