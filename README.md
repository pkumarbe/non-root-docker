# non-root-docker
How a non root user can access docker commands.  

1. Create the docker group.  
   sudo groupadd docker
2. Add your user to the docker group.  
   sudo usermod -aG docker $USER  
3. Activate the changes to groups:  
   newgrp docker   
4.Verify that you can run docker commands without sudo.  
   docker run hello-world  
