## Fork, Clone, Add Remote

> **Note**
>
> For credit, I will check your working branch that you push to GitHub. You should not create a Pull Request this week.
> Enter the URL for your fork and working-branch on a new line in [this document](https://docs.google.com/document/d/1f2dWayE9ZYw8tWVn5I2ccXdyBvKyfHL9SsS_PU73q_E/edit?usp=sharing)
> For example, Sally would add `https://github.com/sallyom/spring-2023/tree/working-branch`

1. Fork the class repository to your GitHub account through the web-based user interface.
    - [Class Repository](https://github.com/DS219/spring-2023).
    - Use the SSH version URL (git@github.com:your-gh-username/spring-2023.git). Otherwise you'll need to provide a username & password to push changes to GitHub.

2. Open a Terminal and clone your forked repository to create a local copy. Run something like the following.
     
    ```bash
    mkdir -p github-repos/DS219 && cd github-repos/DS219
    git clone <paste from github YOUR forked github repository>
    cd spring-2023
    ```

3. You now have a local copy of **your** fork of the class repository. Now add a `git remote` to track the original (upstream) repository.
     
    ```bash
    git remote -v
    # you should see 'origin' as 'git@github.com:DS219/spring-2023.git'
    # now add the 'upstream' remote
    git remote add upstream git@github.com:DS219/spring-2023.git
    ```

4. Add a working branch to your local checkout of DS219/spring-2023 and push it to GitHub.

    ```bash
    git checkout -b working-branch
    # (or) git switch -c working-branch
    ```

5. Add a file to the folder `assignments/feb-15` named `<your-last-name>-<your-first-name>` to this new-branch in your _local checkout of the repository_. Write today's date and time on the file. Then commit this new file and push your working branch to GitHub. 

    ```bash
    git add <your new file>
    git commit -m "<your last name>-feb15"
    git push origin working-branch
    ```
