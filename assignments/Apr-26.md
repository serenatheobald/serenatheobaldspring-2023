## Fork and clone PacMan repository

```
# first, fork https://github.com/font/pacman.git

cd /your/git/repos
git clone git@github.com:yourname/pacman.git
cd pacman
```

## Check out a new branch

```bash
git checkout -b [new-branch]
```

## Build & Run PacMan

* Notice the `LICENSE`. Do you have permission to use this code as you wish?
* Try to run the program locally. The README describes how to do this. Were you successful?
* Look at the Dockerfile. Do you understand what it's doing?
* Build an image and push it to your Docker repository. List your image on the form.
* Run your image. Does it work? What command did you use to run the image?

* `EXTRA CREDIT`: Make a change (any change!) that is visible when the program is run. Build and push that image.
* `EXTRA EXTRA CREDIT`: Configure a database to keep records of games played with best scores. Explain how you did it.

You can use Podman, Docker, or any other container build tool. I'll be using Podman in the examples.
