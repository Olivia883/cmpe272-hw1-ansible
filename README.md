# CMPE 272 - HW1 Ansible (Enterprise Software Plateforms)
## Ansible Web Server Deployment

Used **Ansible** to deploy and un-deploy web server resources on two Ubuntu virtual machines.
Ansible is used to configure both virtual machines, install Nginx, configure the web server to use port **8080**, and deploy a unique web page to each VM.

---
## Assignment Requirements

This project fulfills the following requirements:

1. Configure two virtual machines, **VM1** and **VM2**.
2. Configure Ansible to deploy a web server on VM1 and VM2.
3. Configure both web servers to use port **8080**.
4. VM1 displays:
   `Hello World from SJSU-1`
5. VM2 displays:
   `Hello World from SJSU-2`
6. Both web pages are accessible through a web browser.
7. Include Ansible plays to **deploy** the web server resources.
8. Include Ansible plays to **un-deploy** the web server resources.
9. Document the implementation with screenshots and a demonstration.
10. Store the Ansible code and project documentation in GitHub.

---

## Architecture

```text
                         MacBook
                            |
                            |
                         Ansible
                            |
              +-------------+-------------+
              |                           |
              v                           v
           VM1 (UTM)                   VM2 (UTM)
        Ubuntu Server                Ubuntu Server
              |                           |
           Nginx                        Nginx
          Port 8080                    Port 8080
              |                           |
              v                           v
   Hello World from SJSU-1     Hello World from SJSU-2
