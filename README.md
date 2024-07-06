
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

<p align="center">
  Create droplet ("my-server")<br/>
  Create and configure firewall on DigitalOcean("server-firewall"): <br/>
  set inbound rules<br/>
  set my client PC ip as ssh source so that only my PC can ssh into the server<br/>
  Login to DigitalOcean<br/>
  Select droplet<br/>
  create droplet<br/>
  chose the closest region where you want droplet to be created<br/>
  Select Ubuntu Operating system<br/>
  Select the version (eg. 24.04 (lts)*64)<br/>
  Select CPU options<br/>
  Create droplet<br/>
   My-server has been created
  <img src='./screenshots/1image.png' height="80%" width="80%" alt="Disk Sanitization Steps">

  2. install docker on the server <br/>
     Set up and run jenkins as Docker container<br/>
     ssh into the server (ssh root@publicIP)<br/>
     update the binaries (apt update)<br/>
     install docker (apt install docker.io)
  <img src='./screenshots/2image.png' height="80%" width="80%" alt="Disk Sanitization Steps">
  <img src='./screenshots/3image.png' height="80%" width="80%" alt="Disk Sanitization Steps">

  3. install Jenkins as docker image<br/>
   docker ps<br/>
   login to the jenkins running container (docker exec -it containerId bash)<br/>
   configure firewall custom port and add jenkins container port 8080<br/>
   enter the publicIp of the jenkins server and the port where jenkins is running into the browser<br/>
   (publicIp:port)<br/>
   get the content of the password for jenkins<br/>
   install plugins<br/>
  <img src='./screenshots/4image.png' height="80%" width="80%" alt="Disk Sanitization Steps">

  
    Jenkins image has been pulled from dockerhub and the container is running as well
   <img src='./screenshots/6image.png' height="80%" width="80%" alt="Disk Sanitization Steps">

  
  4. initialize Jenkins <br/>
   <img src='./screenshots/5image.png' height="80%" width="80%" alt="Disk Sanitization Steps">
  
     
  
  
  
  

       

    

</p>




  

 



  





