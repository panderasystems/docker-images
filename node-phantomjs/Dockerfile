FROM circleci/node:8.1

# Upgrade apt-get database & install aws dependencies
RUN sudo apt-get update && sudo apt-get install -y python python-pip libpython-dev
RUN sudo pip install --upgrade awscli

# Install phantomjs dependencies
RUN sudo apt-get install build-essential chrpath libssl-dev libxft-dev -y
RUN sudo apt-get install libfreetype6 libfreetype6-dev -y
RUN sudo apt-get install libfontconfig1 libfontconfig1-dev -y

# Download and install phantomjs
WORKDIR /tmp
ENV PHANTOM_JS phantomjs-2.1.1-linux-x86_64
RUN wget https://bitbucket.org/ariya/phantomjs/downloads/$PHANTOM_JS.tar.bz2
RUN sudo tar xvjf $PHANTOM_JS.tar.bz2

# Link Phantom
RUN sudo mv $PHANTOM_JS /usr/local/share
RUN sudo ln -sf /usr/local/share/$PHANTOM_JS/bin/phantomjs /usr/local/bin

WORKDIR ~
