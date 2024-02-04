# 0x0E. Web stack debugging #1 

<p align="center">
  <img src="https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/271/B4eeypV.jpg" />
</p>

## Resource

- [Resources from Web stack debugging #0](https://github.com/locustbea/alx-system_engineering-devops/tree/main/0x0D-web_stack_debugging_0#resource)


## Tasks

<details>
<summary><a href="./0-nginx_likes_port_80">0. Nginx likes port 80</a></summary><br>
<a href='https://postimages.org/' target='_blank'><img src='https://i.postimg.cc/43fwt3rJ/image.png' border='0' alt='image'/></a>
</details>

<details>
<summary><a href="./1-debugging_made_short">1. Make it sweet and short</a></summary><br>
<a href='https://postimg.cc/dDNKGf46' target='_blank'><img src='https://i.postimg.cc/FsNsX5SM/image.png' border='0' alt='image'/></a>
</details>

# Project: 0x0E. Web stack debugging #1

## Tasks

| Task | File |
| ---- | ---- |
| 0. Nginx likes port 80 | [0-nginx_likes_port_80](./0-nginx_likes_port_80) |
| 1. Make it sweet and short | [1-debugging_made_short](./1-debugging_made_short) |

# 0x0E. Web stack debugging #1
<img src="Web Debugging_1.jpg" />

# Requirements
## General
-  Allowed editors: vi, vim, emacs
-  All your files will be interpreted on Ubuntu 20.04 LTS
-  All your files should end with a new line
-  A README.md file at the root of the folder of the project is mandatory
-  All your Bash script files must be executable
-  Your Bash scripts must pass Shellcheck without any error
-  Your Bash scripts must run without error
-  The first line of all your Bash scripts should be exactly #!/usr/bin/env bash
-  The second line of all your Bash scripts should be a comment explaining what is the script doing
-  You are not allowed to use wget

# Tasks
## 0. Nginx likes port 80
mandatory <br>
Using your debugging skills, find out what’s keeping your Ubuntu container’s Nginx installation from listening on port 80. Feel free to install whatever tool you need, start and destroy as many containers as you need to debug the issue. Then, write a Bash script with the minimum number of commands to automate your fix.

### Requirements:
-  Nginx must be running, and listening on port 80 of all the server’s active IPv4 IPs
-  Write a Bash script that configures a server to the above requirements

### Config Commands
Step 1:
-  curl 0:80
-  ./0-nginx_likes_port_80 > /dev/null 2&>1

Step 2:
-  curl 0:80

Repo:

    GitHub repository: alx-system_engineering-devops
    Directory: 0x0E-web_stack_debugging_1
    File: 0-nginx_likes_port_80


## 1. Make it sweet and short
#advanced <br>
Using what you did for task #0, make your fix short and sweet.

### Requirements:
-  Your Bash script must be 5 lines long or less
-  There must be a new line at the end of the file
-  You must respect usual Bash script requirements
-  You cannot use ;
-  You cannot use &&
-  You cannot use wget
-  You cannot execute your previous answer file (Do not include the name of the previous script in this one)
-  service (init) must say that nginx is not running ← for real

### Config Commands
-  curl 0:80
-  cat -e 1-debugging_made_short | wc -l
-  ./1-debugging_made_short
-  curl 0:80
-  service nginx status

Repo:

    GitHub repository: alx-system_engineering-devops
    Directory: 0x0E-web_stack_debugging_1
    File: 1-debugging_made_short
