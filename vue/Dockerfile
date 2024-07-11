FROM php:8.2-fpm
#NVM install Node
RUN curl -o- 'https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh' | bash
RUN cd ~/../root/.nvm/ && bash nvm.sh && bash -l -c "nvm install 20"
#Node install packages
RUN bash -l -c "npm install -g npm@10.8.1" && \
    bash -l -c "npm install -g @vue/cli"

WORKDIR /app
