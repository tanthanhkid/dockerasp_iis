# HOW TO RUN

* docker build -t dockerasp .
* docker run -d --name dockerasp_env dockerasp

# HOW TO ACCESS WEB

* docker exec dockerasp_env powershell.exe ipconfig
* ==> get the ipv4
