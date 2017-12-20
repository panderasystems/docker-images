## Java JDK v1.8 based on java-8 with python and aws-cli
* Java: 1.8
* Python: latest
* aws-cli: latest
---
# Pull from Docker Hub
`docker pull panderalabs/java-jdk8:latest`
# Build from GitHub
`docker build -t panderalabs/java-jdk8 github.com/panderasystems/java-jdk8`
# Run image
`docker run -it panderalabs/java-jdk8 bash`
# Use as base image
`FROM panderalabs/java-jdk8:latest`
