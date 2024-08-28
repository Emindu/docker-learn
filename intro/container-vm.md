Here’s a Markdown formatted short note based on the provided captions:

```markdown
# Understanding Containers vs. Virtual Machines

## Introduction to Containers
1. **Definition**: When searching for a definition of a container, many compare it to virtual machines.
2. **Comparison**: While there are similarities, containers and virtual machines are fundamentally different.

## Containers as Processes
3. **Concept**: Containers should be viewed as processes running on the host operating system (Linux in this case).
4. **Simplicity**: A container is essentially a restricted process within the host OS, not a virtual machine.

## Starting a Mongo Database
5. **Running Mongo**: We will start a Mongo database container named `mongo` in the background using the Mongo image.
6. **Process Check**: After starting, we can use `docker top` to list processes running inside the container.

## Process Visibility
7. **Single Process**: The MongoDB process (`mongod`) can be observed with its process ID (PID).
8. **Host Visibility**: Since containers are processes on the host OS, standard host tools can also view them.
9. **Process List**: Using a process list command, we can find the `mongod` process running with a unique PID.

## Container Management
10. **Stopping the Container**: If we stop the container, using `docker ps` will show that it is no longer running.
11. **Process Absence**: Running `ps aux` will not display the `mongod` process since the container is stopped.
12. **Searching for Processes**: Using `ps aux | grep mongo` will only show the search command itself, confirming that the process is not running.

## Restarting the Container
13. **Starting the Container**: We can restart the stopped container with `docker start mongo`.
14. **Verification**: Running `docker ps` again will show that the container is back to running.
15. **Process Check Again**: Using `docker top mongo` will reveal that the `mongod` process is running once more.
16. **Process Confirmation**: A subsequent `ps aux | grep mongo` will confirm the visibility of the `mongod` process.

## Conclusion
- Containers are lightweight, isolated processes that run on the host OS, providing a clear distinction from traditional virtual machines. This understanding helps in effectively managing and utilizing containers in development and deployment scenarios.
```

Feel free to use or modify this Markdown note as needed!
