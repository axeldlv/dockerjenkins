# Jenkins 2.91 Docker Image

*In this Dockerfile, i add the library to build docker image.*

Build the image :
```
docker build --rm -t axeldlv/ownjenkins:1 .
```
Launch the jenkins docker :
```
docker run -d -p 49001:8080 -t axeldlv/ownjenkins:1
```
Add a volume :
```
add -v $PWD/jenkins:/var/jenkins_home
```
To use completely java build jenkins, we need to add JDK 8 and Maven 3.5.0
