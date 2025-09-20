# Base image
FROM jenkins/jenkins:alpine3.22-jdk21

# Install docker client
USER root
RUN apk update
RUN apk add --no-cache docker-cli
RUN apk add --no-cache docker-compose 

# Switch back to jenkins user
USER jenkins
