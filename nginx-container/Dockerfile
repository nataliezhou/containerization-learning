# Deploys Nginx server on docker container using Dockerfile
# Run 'docker build . -t <image tag>', 'docker run -d -p 80:80 <image tag>'
# Test that Nginx connection works at localhost

# build from base image ubuntu 18.04
FROM ubuntu:18.04 as ubuntu

# Install nginx
RUN apt-get -y update && apt-get -y install nginx

# Expose port for access 
EXPOSE 80

# Run Nginx server
CMD ["/usr/sbin/nginx", "-g", "daemon off;"]

	
RUN apt-get clean

