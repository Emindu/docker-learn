## Docker Container Monitoring Commands

### Prerequisites
- Basic understanding of how to start a Docker container.

### Commands Overview
In this lecture, we explored several Docker commands to monitor and understand what is happening inside running containers.

1. **Starting Containers**:
   - We began by starting an Nginx container:
     ```bash
     docker container run -d --name nginx nginx
     ```
   - Then, we started a MySQL container with a randomly generated root password:
     ```bash
     docker container run -d --name mysql -e RANDOM_ROOT_PASSWORD=true mysql
     ```

2. **Monitoring Commands**:
   - **`docker container top`**: Lists all processes running inside a container.
     ```bash
     docker container top mysql
     docker container top nginx
     ```
   - **`docker container inspect`**: Provides detailed configuration information about how a container was started, outputting data in JSON format.
     ```bash
     docker container inspect mysql
     ```
   - **`docker container stats`**: Displays real-time performance statistics for running containers, including CPU, memory usage, and more.
     ```bash
     docker container stats
     ```

### Summary
- We used `docker container top` to view running processes, `docker container inspect` to see detailed container configuration, and `docker container stats` to monitor resource usage in real-time.
- These commands are crucial for monitoring containers, especially in production environments where resource management is critical.
