# Mission Reflection

This laboratory activity helped me understand why containerization has become an important part of modern cloud computing. Compared with installing an operating system on a Virtual Machine, starting a Docker container is much faster and requires fewer resources. A VM needs to boot an entire guest operating system before an application can run, while a container can start in seconds because it shares the host operating system kernel. In this activity, the Nginx web server was deployed with only a few Docker commands, which showed how quickly applications can be prepared and tested.

Port mapping using `-p 8080:80` is necessary because the Nginx web server runs on port 80 inside the container, while port 8080 on the host is used to access the service. The mapping connects the host's port 8080 to the container's port 80. Without this mapping, the Nginx service would not be directly accessible through `localhost:8080` from the host environment.

When the `docker rm` command is used, the specified stopped container is permanently removed. Any data stored only inside the container that is not saved using a volume or another external storage method can also be lost. In this activity, removing the `nginx-server` container resulted in the container no longer appearing when `docker ps -a` was executed.

Containerization also changes how software developers and IT operations teams work together. Developers can package applications and their dependencies into containers, while IT and operations teams can deploy the same containers in different environments. This supports DevOps practices by making application deployment more consistent, repeatable, and efficient.

My GitHub portfolio is also evolving as I continue adding new laboratory activities and documenting what I learn. Laboratory 4 added practical experience with Docker and containerization to the previous cloud computing research and infrastructure activities. By keeping the activities organized in separate folders with Markdown documentation and screenshots, my portfolio is becoming a record of both my technical skills and my progress as a cloud computing student.

