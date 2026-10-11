# Laboratory 07: Cloud Operations Engineer

## Mission Overview
Short paragraph: you acted as a Cloud Operations Engineer, checked the host
baseline, deployed an Nginx container, generated traffic, and monitored it
using logs and metrics.

## Objectives
- Establish a host system baseline (RAM, disk, CPU)
- Deploy a containerized web server
- Generate and analyze application logs
- Monitor real-time container resource usage

## Monitoring Commands Executed
| Command | Purpose |
|---|---|
| `free -h` | Check memory usage |
| `df -h /` | Check disk storage |
| `top` | View processes and CPU load |
| `docker run -d --name client-website -p 8080:80 nginx` | Deploy Nginx |
| `docker ps` | Checks the status of running Docker containers. |
| `curl http://localhost:8080` | Simulate user traffic |
| `curl http://localhost:8080/hidden-admin-page` | Tests a nonexistent page and generates a 404 response. |
| `docker logs client-website` | View application logs |
| `docker stats` | View live container metrics |

## Skills Learned

Through this laboratory activity, I learned how to check the health of a Linux server and monitor the resources used by a Docker container. I practiced deploying an Nginx web server, sending HTTP requests, and identifying successful and failed responses. I also learned that application logs help administrators investigate errors, while Docker statistics provide information about CPU and memory consumption. These skills are useful for identifying possible performance problems and understanding how to maintain a reliable web application.
