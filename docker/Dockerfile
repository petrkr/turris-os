FROM ubuntu:trusty
RUN apt-get update && apt-get -y install build-essential bzr cvs gawk flex gettext libncurses5-dev libxml-parser-perl subversion unzip zip findutils zlib1g-dev libssl-dev git-core wget libc6-dev libc6-dev-i386 vim
RUN groupadd -g 2001 build
RUN useradd -m -u 2001 -g 2001 build
RUN echo 'build ALL=(ALL)	NOPASSWD: ALL' >>/etc/sudoers
USER build
WORKDIR /home/build
RUN mkdir share
ENTRYPOINT bash

