## Node.js 8.x based on node/8 with python and aws-cli
* Node: 8.x
* yarn: stable
* Python: latest
* aws-cli: latest
---
# Pull from Docker Hub
`docker pull panderalabs/node-python:latest`
# Build from GitHub
`docker build -t panderalabs/node-python github.com/panderasystems/node-python`
# Run image
`docker run -it panderalabs/node-python bash`
# Use as base image
`FROM panderalabs/node-python:latest`
