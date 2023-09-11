FROM lscr.io/linuxserver/code-server:latest

USER root 

# Install playground-CLI
RUN curl -O https://storage.googleapis.com/artifacts.playground.napptive.dev/installer.sh && bash installer.sh

# Install NodeJS
RUN curl -fsSL https://deb.nodesource.com/setup_current.x | bash - && \
    apt-get install -y nodejs \
    build-essential && \
    node --version && \
    npm --version

RUN mkdir -p /extensions/code-server/extensions && chmod -R  777 /extensions

RUN echo  'export XDG_DATA_HOME=/extensions' >> /etc/profile

RUN useradd -ms /bin/bash coder

ENV XDG_DATA_HOME=/extensions
