# Mission Reflection

Writing the `docker-compose.yml` file made my work as a cloud computing student easier because I did not have to type many commands one by one. Instead, I could put the needed configurations in one file and use Docker Compose to deploy the Nextcloud and MariaDB containers together. This made the process faster and more organized, especially when working with multiple containers.

I also learned that YAML is very sensitive to indentation. If I use the wrong spacing or a Tab instead of spaces, the file may show an error and Docker Compose may not be able to read or run it properly. This taught me to be more careful when writing configuration files because even a small mistake can affect the whole deployment.

We used environment variables such as `MYSQL_PASSWORD` because they allow us to provide important settings to the containers without putting them directly into commands. They also help the application and database communicate with each other correctly. Through this, I understood that environment variables are important when configuring containers.

Deploying Nextcloud felt exciting because I was able to create a working cloud storage system in just a few minutes. At first, I was a little nervous because there were many steps to follow, but seeing the Nextcloud setup page in the browser made me feel that I had successfully completed the deployment.

Since Mission 1, my understanding of Cloud Computing has improved. I learned that cloud computing is not only about using online services but also about managing infrastructure, containers, and configurations. This mission helped me understand how cloud engineers can use automation and Infrastructure as Code to make deployments easier and more efficient.

