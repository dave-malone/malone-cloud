# This is a comment
FROM jenkins:latest
MAINTAINER David Malone <dmalone@pivotal.io>

COPY plugins.txt /usr/share/jenkins/plugins.txt
RUN /usr/local/bin/plugins.sh /usr/share/jenkins/plugins.txt
