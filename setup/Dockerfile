# Base image
FROM jenkins/jenkins:alpine3.22-jdk21

# Install docker client
USER root
RUN apk update && apk add --no-cache docker-cli

# Switch back to jenkins user
USER jenkins
