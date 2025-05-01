FROM jenkins/jenkins:lts

USER root
RUN apt-get update && apt-get install -y nodejs npm && \
    npm install -g newman
USER jenkins
