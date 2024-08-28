## Starting a Nginx Web Server

### `docker container run --publish 80:80 nginx`
- **Description**: Runs a new container from the `nginx` image and maps port 80 of the container to port 80 of the host machine.
- **Usage**: Use this command to start an Nginx web server and access it from your host machine's web browser.

### `docker container run --publish 80:80 --detach nginx`
- **Description**: Runs a new container in detached mode (in the background) from the `nginx` image and maps port 80 of the container to port 80 of the host machine.
- **Usage**: Use this command to start an Nginx web server in the background.

### `docker container ls`
- **Description**: Lists all running containers.
- **Usage**: Use this command to check if your Nginx container is running.

### `docker container stop 690`
- **Description**: Stops the container with ID `690`.
- **Usage**: Use this command to stop a running container.

### `docker container ls -a`
- **Description**: Lists all containers, including stopped ones.
- **Usage**: Use this command to view all containers, both running and stopped.

### `docker container run --publish 80:80 --detach --name webhost nginx`
- **Description**: Runs a new container in detached mode from the `nginx` image, maps port 80 of the container to port 80 of the host machine, and assigns the name `webhost` to the container.
- **Usage**: Use this command to start an Nginx web server with a specific name.

### `docker container logs webhost`
- **Description**: Displays the logs of the container named `webhost`.
- **Usage**: Use this command to view the logs of a specific container.

### `docker container top webhost`
- **Description**: Displays the running processes of the container named `webhost`.
- **Usage**: Use this command to view the processes running inside a container.

### `docker container rm 63f 690 ode`
- **Description**: Removes the containers with IDs `63f`, `690`, and `ode`.
- **Usage**: Use this command to remove one or more stopped containers.

### `docker container rm -f 63f`
- **Description**: Forcefully removes the container with ID `63f`, even if it's running.
- **Usage**: Use this command to remove a running container.
