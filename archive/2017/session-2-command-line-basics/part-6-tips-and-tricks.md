# Part 6: Tips & Tricks

---

#### Better, Faster, Stronger!

Below is a list of more useful stuff and shortcuts. Try them out!

**Commands**:

* `date` - will show you the current system date
* `hostname` - shows the machine name you're currently logged into
* `head` - prints out the first _n_ lines of a file \(defaults to 10\); example: `head -5 file.txt`
* `tail` - similar to head, prints out the last _n_ lines of a file \(also defaults to 10\); example: `tail -5 file.txt`
    {% hint style='tip' %}
`tail -<n>f` will continue to show the last _n_ lines of a file so that if it's updated, the output will be as well.
    {% endhint %}
* `clear`- will clear your terminal
* `whoami` - tells you the username that you're logged in as
* `uptime` - displays how long your machine has been up
* `ping` - checks to see if a reply is received from a remote location
    {% hint style='tip' %}
Example: `ping towel.blinkenlights.nl`
    {% endhint %}
* `history`- lists out the prior history of commands
* `!!` - allows you to repeat the last command ran; you can also append to it like this:
    {% hint style='tip' %}
For example, if the last command you ran was `history`, you could then run `!! | grep cat` and you would get the same output of all of the listed items in history that included the string 'cat'.
    {% endhint %}
* `sudo` - used when elevated permissions are required
    {% hint style='tip' %}
`sudo !!` would append `sudo` to the beginning on the last command ran. This is especially useful when you forget to use elevated, or `sudo`, privileges with a command.
    {% endhint %}

**Get help \(super useful!\)**:

* `man` - shows you the manual or help page of a command, often including syntactical examples
    {% hint style='tip' %}
For example, `man chmod` will give you information on how to use the `chmod` command and what it does.
    {% endhint %}
* `/?`, `--help`, or `-h` - will show help text of a command when added as an option
    {% hint style='tip' %}
To be used in the format `<command> /?`. Example: `grep --help`.
    {% endhint %}

**Moving around at the CLI prompt**:

* Ctrl + U: Clears the line from the cursor point back to the beginning.

* Ctrl + A: Moves the cursor to the beginning of the line.

* Ctrl + E: Moves the cursor to the end of the line.

* Ctrl + R: Allows you to search through the previous commands.

* Ctrl + C: Cancels out of the current command.

**Have some fun!**

Here's a few fun things you can do in the command line:

1. Play a fun game to sharpen your vim skills. Visit https://vim-adventures.com/.

2. Make your computer talk!

    **Mac:** Type `say "Coding and Cocktails is my favorite place"` ![](images/enter.png).
    {% hint style='tip' %}
You can add new voices under System Preferences -> Accessibility -> Speech. If you want to specify a voice, use the syntax  `say -v "Vicki" "hey there pardner"`.
    {% endhint %}

    **Windows:** Enter the following, then ![](images/enter.png).
        ```
        PowerShell -Command "Add-Type –AssemblyName System.Speech; (New-Object System.Speech.Synthesis.SpeechSynthesizer).Speak('what you want your computer to say');"`
        ```

3. Ever wondered what _Star Wars: Episode IV_ would look like in all text? Of course you have!

    **Mac:** Type `telnet towel.blinkenlights.nl` ![](images/enter.png).
    {% hint style='info' %}
The `telnet` command uses a **protocol** that allows you to log in to another remote machine, located in this case at towel.blinkenlights.nl. A protocol is a set of procedures and rules for data transmission.
    {% endhint %}

    **Windows:** Enable telnet by following the video below, then type `winpty telnet towel.blinkenlights.nl` ![](images/enter.png).
    {% hint style='info' %}
The `winpty` command allows Git Bash to properly use the `telnet` command in Windows. You could also run `telnet towel.blinkenlights.nl` in the built-in Windows command prompt to get the same results.
    {% endhint %}

{% raw %}
  <video id="enable-telnet" class="video-js" controls preload="auto" width="900" height="600"
  poster="enable-telnet.jpg" data-setup="{}">
  <source src="videos/enable-telnet.mp4" type='video/mp4'>
  <p class="vjs-no-js">
    To view this video please enable JavaScript, and consider upgrading to a web browser that
    <a href="http://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
  </p>
  </video>
{% endraw %}
