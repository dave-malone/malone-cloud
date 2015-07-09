# This is a comment
FROM tomcat
MAINTAINER David Malone <dmalone@pivotal.io>

RUN git clone git@github.com:dave-malone/personal-financier.git
RUN ./personal-financier/grails war
RUN cp ./personal-financier/target/pf.war /usr/local/tomcat/webapps/

CMD ["catalina.sh", "run"]
