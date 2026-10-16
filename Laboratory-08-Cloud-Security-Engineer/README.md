# Laboratory 08 - Cloud Security Engineer

## Mission Overview

In this laboratory activity, I configured a host-based firewall using UFW to improve the security of an Ubuntu server. I deployed an Nginx web application, checked its availability, and configured firewall rules to allow only the necessary incoming connections.

## Objectives

- Understand the Principle of Least Privilege and the attack surface.
- Configure UFW with a default deny incoming policy.
- Allow SSH and HTTP application traffic on port 8080.
- Verify firewall rules and test the web application using curl.
- Document the security configuration and maintain my GitHub portfolio.

## Commands Executed

**Deploy Nginx**
```bash
docker run -d --name secure-web-app -p 8080:80 nginx
```

**Test the application**
```bash
curl http://localhost:8080/
docker ps
```

**Configure the firewall**
```bash
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
```

**Allow application traffic and verify the rules**
```bash
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned

- Deploying and testing a web server using Docker and Nginx.
- Configuring a Linux host-based firewall using UFW.
- Applying default deny and least-privilege security principles.
- Managing network ports and allowing necessary traffic.
- Documenting technical procedures using Markdown and GitHub.
