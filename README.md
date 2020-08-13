# jenkins-with-docker
A Jenkins docker instance with docker also inside.

## Run

```
docker run -itd --name jenkins -v /var/run/docker.sock:/var/run/docker.sock -v jenkins_home:/var/jenkins_home -v $(which docker):/usr/bin/docker -p 8111:8080 -p 50000:50000 -u root lcaparros/jenkins-with-docker
```