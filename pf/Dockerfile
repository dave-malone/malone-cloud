# This is a comment
FROM tomcat
MAINTAINER David Malone <dmalone@pivotal.io>

RUN apt-get update
RUN apt-get install -y git
RUN apt-get install -y openjdk-7-jdk

RUN git clone https://github.com/dave-malone/personal-financier.git

ENV JAVA_HOME /usr/lib/jvm/java-7-openjdk-amd64

RUN cd ./personal-financier && ./grailsw war
RUN cp ./personal-financier/target/pf.war /usr/local/tomcat/webapps/

CMD ["catalina.sh", "run"]
