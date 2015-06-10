# This is a comment
FROM jenkins:latest
MAINTAINER David Malone <dmalone@pivotal.io>

USER root

RUN apt-get update && apt-get install -y ruby ruby-dev
RUN ruby --version
RUN gem --version
RUN gem install bundler
RUN bundle --version

USER jenkins

COPY plugins.txt /usr/share/jenkins/plugins.txt
RUN /usr/local/bin/plugins.sh /usr/share/jenkins/plugins.txt
