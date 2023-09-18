FROM codercom/code-server:4.9.1

USER root 

# nodejs installation
RUN curl -fsSL https://deb.nodesource.com/setup_current.x | bash - && \
    apt-get install -y nodejs \
    build-essential && \
    node --version && \
    npm --version

RUN mkdir -p /extensions/code-server/extensions && chmod -R  777 /extensions
RUN echo  'export XDG_DATA_HOME=/extensions' >> /etc/profile

USER coder
ENV XDG_DATA_HOME=/extensions
RUN code-server --install-extension eg2.vscode-npm-script