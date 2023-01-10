# Jenkins

Setup Jenkins using docker
https://github.com/jenkinsci/docker/blob/master/README.md
```
docker run --name jenkins -p 8080:8080 -p 50000:50000 --restart=on-failure jenkins/jenkins:lts-jdk11
```

docker exec <container_name> cat /var/jenkins_home/secrets/initialAdminPassword

docker logs <container_name>