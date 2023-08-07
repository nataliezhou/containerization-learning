# Deploys Redis on Docker container using Dockerfile
# Inside ./redis-container, run 'docker build . -t <image tag>', 'docker run -d -p 6379:6379 --name <container name> <image tag>'
# Test Redis connection by running 'docker exec -it myredis sh' to enter shell and run 'redis-cli ping'

# build from base image ubuntu 18.04
FROM ubuntu:18.04 as ubuntu
RUN apt-get update && apt-get install -y redis-server
EXPOSE 6379
ENTRYPOINT ["/usr/bin/redis-server"]
# build instruction
RUN echo "Run 'docker exec -t <container-name> sh' to enter Redis CLI shell"
RUN apt-get clean
