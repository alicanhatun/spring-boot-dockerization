## **Spring Boot Dockerization**

* **FROM** 
    * The base image for building a new image. This command must be on top of the dockerfile. 
* **MAINTAINER** 
    * Optional, it contains the name of the maintainer of the image. 
* **RUN** 
    * Used to execute a command during the build process of the docker image. 
* **ADD** 
    * Copy a file from the host machine to the new docker image. There is an option to use a URL for the file, docker will then download that file to the destination directory. 
* **ENV** 
    * Define an environment variable. CMD Used for executing commands when we build a new container from the docker image. 
* **ENTRYPOINT** 
    * Define the default command that will be executed when the container is running. 
* **WORKDIR** 
    * This is directive for CMD command to be executed. 
* **USER** 
    * Set the user or UID for the container created with the image. 
* **VOLUME** 
    * Enable access/linked directory between the container and the host machine. Now let's start to create our first dockerfile.
    
    
**COMMANDS**
* docker build -f Dockerfile -t springbootdockerization .
* docker run -p 8080:8080 -d springbootdockerization

