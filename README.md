# spring-boot-demo-jenkins
    admin
    9b56645cbf5e490780b373f2dd147d3b

docker container run  \  
    -p 8086:8080 \
    -v jenkinsvol:/var/jenkins_home \
    --name jenkins-local1 \
    jenkins/jenkins

make some changes
