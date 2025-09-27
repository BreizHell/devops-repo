# Base image
FROM jenkins/jenkins:alpine3.22-jdk21

# Install docker client
USER root
RUN apk update
RUN apk add --no-cache docker-cli
RUN apk add --no-cache docker-compose 

# Create maven repository with ownership to jenkins user

RUN mkdir -p --mode=755 /var/jenkins_home/.m2/repository
RUN chown -R jenkins:jenkins /var/jenkins_home/.m2/repository

# Switch back to jenkins user
USER jenkins
