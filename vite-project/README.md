# command run with root in jenkins
- docker run -d --name jenkins-docker \
  -u root \
  -p 8080:8080 -p 50000:50000 \
  -v jenkins_home:/var/jenkins_home \
  jenkins/jenkins
- docker exec -it jenkins-docker bash
- apt update
- apt install -y docker.io
- export DOCKER_HOST=tcp://host.docker.internal:2375

