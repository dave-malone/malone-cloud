# This is a comment
FROM tomcat
MAINTAINER David Malone <dmalone@pivotal.io>

RUN which java

RUN apt-get update
RUN apt-get install -y git

RUN git clone https://github.com/dave-malone/personal-financier.git
RUN ./personal-financier/grailsw war
RUN cp ./personal-financier/target/pf.war /usr/local/tomcat/webapps/

CMD ["catalina.sh", "run"]
