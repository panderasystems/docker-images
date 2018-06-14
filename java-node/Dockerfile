FROM circleci/openjdk:8-jdk

RUN curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
RUN \
    sudo apt-get update && \
    sudo apt-get install -y nodejs && \
    sudo npm install -g yarn
