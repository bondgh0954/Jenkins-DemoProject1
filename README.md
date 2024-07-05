
<h1>Jenkins-DemoProject1</h1>

<h2>Project Description</h2>
 1. Create an Ubuntu server on DigitalOcean<br/>
 2. Set up and run jenkins as Docker container<br/>
 3. initialize jenkins<br/>
<br />


<h2>Technologies used</h2> 
- <b>Jenkins</b> <br/>
- <b>Docker</b> <br/>
- <b>DigitalOcean</b> <br/>
- <b>Linux</b> <br/>

<h2>Detailed Description of Project </h2>

<p right="center">
  Create droplet ("my-server")<br/>
  Create and configure firewall on DigitalOcean("server-firewall"): <br/>
  set inbound rules<br/>
  set my client PC ip as ssh source so that only my PC can ssh into the server<br/>
  <img src='./screenshots/1image.png' height="80%" width="80%" alt="Disk Sanitization Steps">

  install docker on the server <br/>
  <img src='./screenshots/2image.png' height="80%" width="80%" alt="Disk Sanitization Steps">
  <img src='./screenshots/3image.png' height="80%" width="80%" alt="Disk Sanitization Steps">

  install Jenkins as docker image<br/>
  <img src='./screenshots/4image.png' height="80%" width="80%" alt="Disk Sanitization Steps">

  configure firewall custom port and add jenkins container port 8080
  copy public IP and jenkins port and start jenkins in the browser
  
  
  
  

       Login to DigitalOcean
       Select droplet
       create droplet
       chose the closest region where you want droplet to be created
       Select Ubuntu Operating system
       Select the version (eg. 24.04 (lts)*64)
       Select CPU options
       Create droplet
       Create and configure firewall
<img src='./src/image1.png' height="80%" width="80%" alt="Disk Sanitization Steps">


<br />
<br />

    2. Set up and run jenkins as Docker container
     ssh into the server (ssh root@publicIP)
     update the binaries (apt update)
     install docker (apt install docker.io)
     install jenkins as a container
       docker run -p 8080:8080 -p 50000:50000 -d -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts
<img src='./src/image2.png' height="80%" width="80%" alt="Disk Sanitization Steps">

3. initialize jenkins
    docker ps
    login to the jenkins running container (docker exec -it containerId bash)
    enter the publicIp of the jenkins server and the port where jenkins is running into the browser
    (publicIp:port)
    get the content of the password for jenkins
    install plugins
<img src='./src/image3.png' height="80%" width="80%" alt="Disk Sanitization Steps">
    

</p>




  

 



  





