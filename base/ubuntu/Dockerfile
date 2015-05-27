FROM ubuntu:14.10
MAINTAINER  Paddy Lin <dragon270329@gmail.com>

# Add useful packages
RUN DEBIAN_FRONTEND=noninteractive apt-get update
RUN DEBIAN_FRONTEND=noninteractive apt-get -y install curl bash-completion vim-tiny supervisor wget

# Setup root password for login process
RUN echo root:root | chpasswd

# Language setup
RUN locale-gen zh_TW zh_TW.UTF-8 en_US.UTF-8
RUN update-locale LANG=en_US.UTF-8

# Common alias
RUN alias ls='ls --color=auto'
RUN alias ll='ls -halF'
