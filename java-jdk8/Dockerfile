FROM circleci/openjdk:8-jdk

RUN \
# must install libpython-dev as per https://github.com/aws/aws-cli/issues/2290
 sudo apt-get update && \
 sudo apt-get install -y python python-pip libpython-dev && \
 sudo pip install --upgrade awscli
