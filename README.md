# ENV
## install JDK
``` sh
 sudo apt-get install openjdk-17-jdk
```
## download jenkin GPG key (A GPG key (GNU Privacy Guard key) is a cryptographic key used for securing communications and verifying the integrity and authenticity of software packages and other digital data)
``` 
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
```
## Adding the Jenkins Package Repository
``` sh
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/" | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
```
## update
```
sudo apt update
```
# install jenkins
``` 
sudo apt-get install jenkins
```
