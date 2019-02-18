# jenkins-please
This Dockerfile will build a Docker container image with Jenkins and Docker CE.

Build it like this:
```
docker image build -t jenkins-please .
```
Run it like this:
```
docker run -d --name jenkins-please -p 80:8080 -v </host/path/to/jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock jenkins-please
```
