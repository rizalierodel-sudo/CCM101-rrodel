# Laboratory 07 – Reflection

A host machine can still have resource issues even if its containers are running properly. This is because containers share the resources of the host machine, such as memory, CPU, and disk space. If too many resources are being used, the host may become slow. I learned that it is important to check the host's resources and not just the status of the containers.

If a customer reports a login problem, I would use `docker logs` to check what is happening inside the application. I would look for error messages or failed requests that might be related to the problem. This would help me understand the possible cause and know what needs to be checked next.

Logs show the events and errors that happen in an application, while metrics show numbers about its performance and resource usage. In our activity, I used `docker logs` to check website requests and the 404 error. I also used `docker stats` to see the CPU, memory, and network usage of the container. Both are helpful because they provide different information when checking for problems.

An enterprise can use monitoring tools like Prometheus and Grafana to monitor many containers at the same time. These tools help collect and display information about container performance and resource usage. Instead of checking each container one by one, engineers can use dashboards to see if something is wrong. This makes monitoring easier when handling many containers.

This laboratory helped me become more familiar with Linux commands and Docker. I practiced checking memory and disk usage, running an Nginx container, testing a website using `curl`, and checking logs and container statistics. I also learned that a 404 error means the requested page cannot be found. Overall, the activities helped me understand how these commands can be used to monitor applications and identify possible problems.


