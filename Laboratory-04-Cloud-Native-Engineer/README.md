# Laboratory 04 - The Cloud-Native Engineer

## Mission Overview

This laboratory activity introduced the concepts of cloud-native engineering, containerization, and Docker. The activity focused on understanding the differences between traditional Virtual Machines (VMs) and containers and demonstrating how Docker can be used to deploy a web server quickly. Using the KillerCoda Ubuntu environment, an Nginx web server was deployed, tested, stopped, and removed using Docker commands.

## Objectives

At the end of this laboratory activity, the following objectives were completed:

* Differentiate between Virtual Machines and containers.
* Access a Docker-enabled Linux environment using KillerCoda.
* Execute fundamental Docker CLI commands.
* Pull and run an Nginx container.
* Map a host port to a container port.
* Test a containerized web server using `curl`.
* Manage the lifecycle of a Docker container.
* Document Docker operations using Markdown.
* Maintain an organized GitHub Cloud Computing portfolio.

## Docker Commands Executed

### Checkpoint 3 - Verify Docker

```bash
docker --version
```

Displays the installed Docker version.

```bash
docker info
```

Displays information about the Docker client and server environment.

### Checkpoint 4 - Deploy Nginx

```bash
docker pull nginx
```

Downloads the official Nginx image from Docker Hub.

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

Runs the Nginx container in detached mode and maps host port 8080 to container port 80.

```bash
curl http://localhost:8080
```

Sends an HTTP request to the Nginx server and verifies that it is working.

### Checkpoint 5 - Container Lifecycle

```bash
docker ps
```

Lists currently running containers.

```bash
docker stop nginx-server
```

Stops the running Nginx container.

```bash
docker ps -a
```

Displays all containers, including stopped containers.

```bash
docker rm nginx-server
```

Removes the stopped Nginx container.

```bash
docker ps -a
```

Verifies that the container has been completely removed.

## Skills Learned

Through this laboratory activity, I learned how containers differ from Virtual Machines and why containers are useful for cloud-native applications. I also learned how to use basic Docker CLI commands to pull images, create and run containers, test applications, stop containers, and remove containers. The activity also improved my understanding of port mapping and how a web service inside a container can be accessed from the host system. In addition, I gained experience in documenting technical procedures and maintaining evidence in a GitHub portfolio.

## Challenges Encountered

One challenge was understanding the different stages of the Docker container lifecycle and remembering which commands should be used to check, stop, and remove a container. Another challenge was understanding how port mapping works, particularly the meaning of `-p 8080:80`. The KillerCoda environment made it possible to practice these commands without installing Docker directly on my personal computer. By following the commands step by step and checking the terminal output, I

