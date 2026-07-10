1. Once you have installed pre-requisites on your Vm instance you can clone the repository using below command:

   git clone https://github.com/SThunderz108/Floci.git

2. Move to Floci directory on your terminal you can find docker compose yaml .

   [ubuntu@jump01]$ cd Floci/docs/

3. Now run docker compose
  
   [ubuntu@jump01]$docker compose up -d

Note : It will spawn 2 docker containers Floci & Floci-Ui 

4. Verify docker containers using below command, you should see similar output.

   ubuntu@jump01:~/Floci/docs$ docker ps
   CONTAINER ID   IMAGE                          COMMAND                  CREATED       STATUS                PORTS                                         NAMES
   d1ed31f02340   floci/floci-ui:latest          "./server"               2 days ago    Up 2 days             0.0.0.0:8080->4500/tcp, [::]:8080->4500/tcp   floci-ui
   24eeb762585c   floci/floci:latest             "/usr/local/bin/dock…"   4 days ago    Up 2 days (healthy)   0.0.0.0:4566->4566/tcp, [::]:4566->4566/tcp   floci

5. Once you have verified docker containers are up & running you can go to web browser enter your ec2 instance public ip:8080

 
  
  

