# Docker Deep Dive: From Container Creation to Cloud Deployment

This repository (or project) chronicles a hands-on exploration into Docker, covering fundamental concepts, practical container management, and pushing images to cloud registries.

## Overview

This project aims to demonstrate:
* The core differences between bare metal, virtualization, and containerization.
* Practical steps to create and customize Docker containers.
* How to manage and push Docker images to both Docker Hub and Amazon Elastic Container Registry (ECR).
* A review of essential Docker commands.

## Key Learnings & Accomplishments

### Understanding the Fundamentals
Gained clarity on the key differences between:
* **Bare Metal**: Physical hardware without virtualization, offering speed but lacking flexibility.
* **Virtualization**: Uses a hypervisor to run multiple Virtual Machines (VMs), each with its own OS, providing flexibility but using more resources.
* **Containerization**: Runs multiple lightweight applications (containers) on a shared OS, making them faster, resource-efficient, and ideal for microservices and scalable cloud applications.

### Hands-on with HTTPD Containers
Successfully created and customized an `httpd` (Apache) container:
* Pulled the `httpd` image from DockerHub and created a container named `apacheserver`.
* Entered the `apacheserver` container.
* Created `home.html` and `about.html` pages inside the container's `htdocs` directory.
* Accessed both `home.html` and `about.html` from a web browser.

### Image Management & Cloud Push

#### Docker Hub
* Committed changes from the `apacheserver` container to create a new Docker image.
* Logged into Docker Hub from the terminal.
* Pushed the newly created image to a Docker Hub repository.

#### Amazon ECR
* Created a public repository in AWS ECR.
* Logged into ECR from the terminal using AWS CLI.
* Tagged the local Docker image for ECR.
* Pushed the image to the created Amazon ECR repository.

### Essential Docker Commands
Reviewed and practiced a comprehensive list of commonly used Docker commands, including:
* `docker --version`: Check Docker installation and version.
* `docker pull <imagename>`: Pull an image from Docker Hub.
* `docker images`: List local Docker images.
* `docker run`: Create and run a container from an image.
* `docker exec -it <cont-name> /bin/bash`: Enter a container in interactive mode.
* `docker ps -a`: List all running containers.
* `docker stop <cont-name>`: Stop a running container.
* `docker start <cont-name>`: Start a stopped container.
* `docker rm <cont-name>`: Remove a stopped container.
* `docker rmi <imagename>`: Remove an image.
* `docker volume ls`: List Docker volumes.
* `docker volume create <name>`: Create a Docker volume.
* `docker network ls`: List Docker networks.
* `docker network create <network-name> --driver <driver-name>`: Create a Docker network.
* `docker inspect <object>`: Inspect Docker objects (container, image, network, volume).
* `docker tag <source-image> <target-image:tag>`: Tag an existing image.
* `docker push <imagename>`: Push an image to a repository.
* `docker login`: Log in to Docker Hub or other registries.

## Conclusion
Docker is a powerful and incredibly useful tool for modern software development and deployment. This hands-on experience has solidified my understanding of containerization principles and practical Docker operations.
