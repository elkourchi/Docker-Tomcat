# Docker-Tomcat

## Dockerfile to setup Tomcat container

### The instructions :

    Pull centos from dockerhub (FROM)
    Install java (RUN)
    Create/opt/tomcat directory (RUN)
    Change work directory to/opt/tomcat (WORKDIR)
    Download tomcat packages (ADD)
    Extract tar.gz file (RUN)
    Rename to tomcat directory (RUN)
    Tell to docker that it runs on port 8080 (EXPOSE)
    host a web app (COPY)
    Start tomcat services (CMD)

### To build an image from this Dockerfile we use the command :

    docker build -t [name] -f [dockerfile path]

### To run a container from this image we use :
    docker run -d --name [container-name] -p 8080:8080 [image-name]




