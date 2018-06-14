## Node.js 8.x based on node/8 with Java 8 JRE
* Java: 1.8
* Node: 8.x
* yarn: stable
---
# Pull from Docker Hub
`docker pull panderalabs/java-node:latest`
# Build from GitHub
`docker build -t panderalabs/java-node github.com/panderasystems/java-node`
# Run image
`docker run -it panderalabs/java-node bash`
# Use as base image
`FROM panderalabs/java-node:latest`
