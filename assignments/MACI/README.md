# Bash 2048 Game Containerized


## Description
The script runs a simple version of the game 2048 in the terminal. The game is played by using the arrow keys or WASD to move the tiles. The goal is to stack the tiles containing powers of 2 until you reach 2048. The game ends when you reach 2048 or when there are no more possible moves. The script is written in bash commands. 

Credit to **JosefZIla** on GitHub for the original script. I modified the script to run in a container.

[Link to original script](https://github.com/JosefZIla/bash2048)

## Building
To build the container, run the following command in the directory containing the Dockerfile:
```
podman build -t 2048 
```
or 
```
docker build -t 2048
```

You can pull the container directly from Docker Hub using the following command:
```
podman pull docker.io/markmaci/2048
```
or
```
docker pull docker.io/markmaci/2048
```

## Running
Since the game is played in the terminal, you must run the container in interactive mode. To do this, run the following command:
```
podman run -it 2048
```
or
```
docker run -it 2048
```
