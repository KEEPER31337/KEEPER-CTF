FROM ubuntu:18.04

# RUN apt update && apt install xinetd -y

RUN mkdir /home/keeper && \
    mkdir /home/keeper/bin

RUN useradd -U -u 999 -d /home/keeper -l keeper

RUN ln -s /bin/ls /home/keeper/bin/ls && \
    ln -s /bin/cat /home/keeper/bin/cat && \
    ln -s /usr/bin/clear /home/keeper/bin/clear

COPY .bashrc /home/keeper/.bashrc

USER keeper

WORKDIR /home/keeper
