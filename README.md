### kafka-spring-samples

- Support Standard Markdown / CommonMark and GFM(GitHub Flavored Markdown);
This Project is created for trying the Kafka Integration with Spring using Docker in local. This project is intended for local execution and strictly for learning purposes only.


### Pre requisites and local setup information
- Make sure you install JDK 11 and above.
- Install Docker Desktop in either Windows or Linux

#### Docker Desktop setup in Linux ( This steps only applicable to Linux Users)
- Docker provides a convenient script for installing the software in Linux. Here is the command you need to run to install Docker.

  ` curl -fsSL https://get.docker.com -o get-docker.sh`
  ` sudo sh get-docker.sh`
- After the install, download the platform specific docker desktop version from docker website
https://docs.docker.com/desktop/install/linux-install/

Since I am using a Debian based Pop OS, I downloaded the  debian package. <br>
`sudo apt-get install ./docker-desktop-4.26.1-amd64.deb`

- Next we need to add some privillages to enable file sharing <br>
` grep "$USER" /etc/subuid >> /dev/null 2&>1 || (echo "$USER:100000:65536" | sudo tee -a /etc/subuid)` <br>
 `grep "$USER" /etc/subgid >> /dev/null 2&>1 || (echo "$USER:100000:65536" | sudo tee -a /etc/subgid)` <br>
- After this, you can check the program files to find the Docker Desktop application and start it.
