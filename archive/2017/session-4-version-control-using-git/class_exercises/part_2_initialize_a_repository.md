### Part 2: Initialize a Repository {#part-2-initialize-a-repository}

1. In Git Bash or iTerm2, make sure you're still in the FirstRepo folder and type `mkdir ../AnotherDir` create another directory nside your _VersionControl_ directory.

2. Type `cd ../AnotherDir` to move into this directory.

    {% hint style='tip' %}
The `../` is telling your computer to look up one level to the parent directory (_VersionControl_) before looking for that _AnotherDir_ directory.
    {% endhint %}

4. Type `ls -la` (remember this from last month?) to view the files in the folder.

5. Type `git init` to initialize your repository.  

6. Type `ls -la` and notice the _.git_ folder that the `git init` command created.

7. In Google Chrome, navigate to [GitHub](https://github.com).

8. In the upper right corner, click on the `+` button and choose `New Repository`.
    ![](/images/createrepo.png)

9.  Give your repository a name, like MyFirstRepo.

10.  Give it a description, and click the checkbox next to `Initialize this repository with a README`.

    {% hint style='tip' %}
You can ignore the `Add .gitignore` and `Add a license` dropdowns for the time being.  You won't need them for what we are doing this evening.
    {% endhint %}

11.  Click `Create Repository`.

**Congratulations! Have a drink! In part 2, you created two repositories and established your presence on GitHub!**

{% hint style='tip' %}
Unless you decide to purchase a paid GitHub account (not necessary for what we do) all of your repositories are automatically publicly searchable.
{% endhint %}
