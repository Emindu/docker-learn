
# Docker Commands Overview

## Check Our Docker Install and Config

### `docker version`
- **Description**: Displays the version of Docker installed on your system, including the client and server versions.
- **Usage**: Run this command to verify that Docker is installed and to check for updates.

### `docker info`
- **Description**: Provides detailed information about the Docker installation, including the number of containers, images, storage driver, and more.
- **Usage**: Use this command to get insights into your Docker environment, such as the system architecture and resource usage.

### `docker`
- **Description**: The base command for Docker CLI. Running `docker` without any arguments displays a list of available commands and options.
- **Usage**: Use this command to explore Docker's capabilities and find commands you might want to use.

### `docker container run`
- **Description**: Creates and starts a container from a specified image. This command can include options for setting environment variables, ports, and more.
- **Usage**: Example: `docker container run -d -p 80:80 nginx` to run an Nginx server in detached mode.

### `docker run`
- **Description**: A shorthand for `docker container run`. It performs the same function of creating and starting a container from an image.
- **Usage**: Example: `docker run -it ubuntu bash` to run an interactive Ubuntu container with a bash shell.
