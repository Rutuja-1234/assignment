# assignment
1.  Create a dockerfile  to  build nodejs image containing your project in work directory 

2. Build an image of nodejs by using command given below 
    
   docker build -t  nodejs . -f  dockerfile


3. Then hit the command  given below to check docker image of nodejs .
   
   docker images

4. Download mysql image by using command
   
   docker pull mysql 

5. Build an image of mongodb by using command given below 
  
    docker build -t mongo . -f dockerfile

6.  Create a yaml  to run three containers of nodejs, mongodb and mysql 
Please check the docker-compose.yml file for services to create in docker-compose.

7. TO run yaml file, hit the command
    
    docker-compose up -d

8. Check the status of containers using command

    docker-compose ps

9. Check the IP address of app container using 

    docker inspect node

10. Copy the IP address.

11. Check the output on browswer using url

       IPAddress:51005/documentation

PS: If swagger UI is not visible then try running these commands to get hapi swagger running inside your nodejs container
	npm install @hapi/inert --save
	npm install @hapi/vision --save

