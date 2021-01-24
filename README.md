# HOW TO RUN

* docker build -t dockerasp .
* docker run -d --name dockerasp_env dockerasp

# HOW TO ACCESS WEB

* docker exec dockerasp_env powershell.exe ipconfig
* ==> get the ipv4

# PUSH TO AWS ECR

* aws ecr get-login-password --region ap-southeast-1 | docker login --username AWS --password-stdin 188038744485.dkr.ecr.ap-southeast-1.amazonaws.com
* docker tag dockerasp:latest 188038744485.dkr.ecr.ap-southeast-1.amazonaws.com/docker_asp:latest
* docker push 188038744485.dkr.ecr.ap-southeast-1.amazonaws.com/docker_asp:latest