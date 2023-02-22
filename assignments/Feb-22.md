## Add a new commit and open a Pull Request

> **Note**
> At the end of this assignment, you should have an open Pull Request. Your Pull Request will be listed [here](https://github.com/DS219/spring-2023/pulls).
> Good luck, ask questions!

This assignment assumes you are working from your terminal and from the directory where this repository is checkout out.
Also, you should be working in a branch other than the main branch. `working-branch` is the name of the branch used here.

1. Make sure you are working from `working-branch`
     
    ```bash
    git checkout working-branch
    # you should already have this branch created, but if not then 'git checkout -b working-branch'
    ```

2. Add a new directory named with your last name and an executable file to this branch.
     
    ```bash
    mkdir assignments/YOUR-LAST-NAME
    ```
    Add a file to this directory using whatever text editor you have set up
    This file should be executable, like the [`joke.sh`](https://raw.githubusercontent.com/DS219/spring-2023/main/joke.sh) file you created in the Feb 8 assignment.
    Create a simple python script, shell command, or anything else that does something.
    Name the file after what it does - for example, `joke.sh` or `hello-world.py`


3. At the top of the file, add a comment that explains what the script does, and how to run it. For example

    ```bash
    # This script downloads and prints a joke from the public site "https://icanhazdadjoke.com"
    # To run this file, type ./joke.sh from this folder. 
    ```

4. Commit the new folder and file

    ```bash
    git add . 
    git commit -m "<your last name>-added an executable file"
    git push origin working-branch
    ```

5. Finally, go to the GitHub UI and open a Pull Request to the DS219/spring-2023 repository!
