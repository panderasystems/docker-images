FROM circleci/openjdk:8-jdk

RUN \
# must install libpython-dev as per https://github.com/aws/aws-cli/issues/2290
 sudo apt-get update && \
 sudo apt-get install -y python python-pip libpython-dev && \
 sudo pip install --upgrade awscli

RUN curl https://releases.hashicorp.com/terraform/0.11.5/terraform_0.11.5_linux_amd64.zip -o ~/terraform.zip \
  && sudo unzip ~/terraform.zip -d /usr/bin \
  && rm ~/terraform.zip
