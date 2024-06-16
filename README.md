# Jenkins-DemoProject1
# Install Jenkins on DigitalOcean

# Technologies used:
   Jenkins
   Docker
   DigitalOcean
   Linux

# Project Description
  1. Create an Ubuntu server on DigitalOcean
  2. Set up and run jenkins as Docker container
  3. initialize jenkins

#  Detailed Description of steps

   1. Create an ubuntu server on DigitalOcean

       Login to DigitalOcean
       Select droplet
       create droplet
       chose the closest region where you want droplet to be created
       Select Ubuntu Operating system
       Select the version (eg. 24.04 (lts)*64)
       Select CPU options
       Create droplet
       Create and configure firewall

2. Set up and run jenkins as Docker container
     ssh into the server (ssh root@publicIP)
     update the binaries (apt update)
     install docker (apt install docker.io)
     install jenkins as a container
       docker run -p 8080:8080 -p 50000:50000 -d -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts

3. initialize jenkins
    docker ps
    login to the jenkins running container (docker exec -it containerId bash)
    enter the publicIp of the jenkins server and the port where jenkins is running into the browser
    (publicIp:port)
    get the content of the password for jenkins
    install plugins

