
In order to build and then run this Docker container, open a terminal / command window, navigate to this directory, and execute the following commands:

```
docker build -t malone-cloud/jenkins:latest . 

docker run -i -t -p 8080:8080 -v ~/jenkins_home:/var/jenkins_home malone-cloud/jenkins
```

Assuming that you are using boot2docker to run Docker on your own machine, you will need to obtain the IP address of the Vagrant VM in order to access Jenkins. This can be obtained by executing `boot2docker ip`, which typically defaults to 192.168.59.103. Then, you would be able to access Jenkins in your browser via the URL [http://192.168.59.103:8080/](http://192.168.59.103:8080/)
