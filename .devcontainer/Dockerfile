FROM mcr.microsoft.com/devcontainers/base:ubuntu

RUN curl -s "https://get.sdkman.io" | bash
RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
RUN apt-get update && apt-get install -y maven
RUN apt-get update && apt-get install -y docker.io

ENV NVM_DIR=/root/.nvm
ENV SDKMAN_DIR=/root/.sdkman

RUN echo "source $SDKMAN_DIR/bin/sdkman-init.sh" >> ~/.bashrc
RUN echo "export NVM_DIR=\"$HOME/.nvm\"" >> ~/.bashrc
RUN echo "[ -s \"$NVM_DIR/nvm.sh\" ] && \. \"$NVM_DIR/nvm.sh\"" >> ~/.bashrc
