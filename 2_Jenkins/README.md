# Jenkins


## Installation
1. Build a image
```
docker image build -t jenkins_lab .
```

2. Run Jenkins using built image
```
docker run --name jenkins -p 8080:8080 -p 50000:50000 --restart=on-failure jenkins_lab
```

3. Setup Jenkins and test
docker exec <container_name> cat /var/jenkins_home/secrets/initialAdminPassword
or
docker logs <container_name>




https://github.com/jenkinsci/docker/blob/master/README.md