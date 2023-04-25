# Tic-Tac-Toe game!
## Pre-Reqs
Before getting started with running the game, you need to have Podman or Docker installed on your computer. Then you also want to have a DockerHub account to be able to pull the image.

## About
This game is basically a containerized game of tic-tac-toe from the github repository https://github.com/AshutoshNirkhe/tic-tac-toe/blob/master/tic-tac-toe.sh. This not my script and I have just containerized it. 

## How to Build
To build the game, you need to create a Containerfile in the same directory of the script. Then add this code,
``` 
FROM fedora 
WORKDIR mydir
ADD tick-tack-toe.sh /mydir
RUN chmod +x /mydir/tick-tack-toe.sh
RUN dnf install -y ncurses
CMD ./tick-tack-toe.sh  

```

## Steps to Run
- First, login to your dockerhub account using the command 
` podman login docker.io `
or
`docker login docker.io`

- Second, you want to run the command 
`podman pull tick-tack`
or 
`docker pull tick-tack `


- Lastly, run `podman run -it tick-tack` or `docker run -it tick-tack` if using Docker, and play the game!

Hope you enjoy!