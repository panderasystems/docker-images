FROM node:8

RUN \
# must install libpython-dev as per https://github.com/aws/aws-cli/issues/2290
 apt-get update && \
 apt-get install -y python python-pip libpython-dev && \
 pip install --upgrade awscli
