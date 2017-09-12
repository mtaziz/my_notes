# BUILD

    # Build an image from the Dockerfile in the current directory and tag the image
    docker build -t myapp:1.0 .
    
    # List all images that are locally stored with the Docker engine
    docker images
    
    # Delete an image from the local image store
    docker rmi alpine:3.4

# RUN

    docker run
    remove container automatically after it exits
    connect the container to terminal
    name the container
    expose port 5000 externally and map to port 80
    create a host mapped volume inside the container
    the image from which the container is instantiated
    the command to run inside the container
    Stop a running container through SIGTERM
    docker stop web
    Stop a running container through SIGKILL
    docker kill web
    Create an overlay network and specify a subnet
    docker network create --subnet 10.1.0.0/24
    --gateway 10.1.0.1 -d overlay mynet
    List the networks
    docker network ls
    List the running containers
    docker ps
    Delete all running and stopped containers
    docker rm -f $(docker ps -aq)
    Create a new bash process inside the container and connect
    it to the terminal
    docker exec -it web bash
    Print the last 100 lines of a container’s logs
    docker logs --tail 100 web
