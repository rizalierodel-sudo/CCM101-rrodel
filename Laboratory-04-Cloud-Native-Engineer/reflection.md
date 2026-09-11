# Mission Reflection

This laboratory activity helped me understand the difference between using a Virtual Machine and a Docker container. When using a Virtual Machine, installing an operating system and setting up the environment can take more time because the VM needs its own operating system and resources. In comparison, a Docker container can start in just a few seconds because it shares the host operating system. I noticed this during the activity when I was able to run the Nginx web server with only a few Docker commands.

Port mapping, such as `-p 8080:80`, is necessary because it allows us to access the web server running inside the container from the host machine. Port 8080 is the port we used on the host, while port 80 is the port used by Nginx inside the container. Without the port mapping, it would be harder to access the Nginx web server through the host.

I also learned that when we use `docker rm`, the container itself is deleted. Any data that was stored only inside the container can also be lost after the container is removed. This is why important data should be stored using volumes or other storage methods instead of relying only on the container.

Containerization can also change how developers and IT operations teams work together. Developers can create applications in containers with the needed environment, while IT teams can deploy the same containers without setting everything up again. This can make the process faster and reduce problems caused by differences between development and production environments.

Lastly, my GitHub portfolio is slowly becoming more organized and complete. I am adding my laboratory activities, documentation, screenshots, and the commands I used. This activity also helped me see that a portfolio is not only about submitting requirements, but also about keeping a record of the skills and tasks I have learned throughout the course.
