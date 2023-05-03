FROM fedora:latest
WORKDIR app
ADD bash2048.sh /app
RUN chmod +x /app/bash2048.sh
RUN dnf install -y ncurses
CMD ./bash2048.sh