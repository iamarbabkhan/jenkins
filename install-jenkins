### Install Jenkins on ec2 aws
1. Create ec2 on aws
2. EC2 Instances - Security - edit inbound rules - all traffic - 8080
3. http://ip:8080

pre-requisites: java(jdk)
* `sudo apt update
sudo apt install openjdk-11-jre`
* `java -version`
* `curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins`
* `sudo cat /var/lib/jenkins/secrets/initialAdminPassword`
* `sudo apt update
sudo apt install docker.io`
* sudo su - 
usermod -aG docker jenkins
usermod -aG docker ubuntu
systemctl restart docker`
* `http://<ec2-instance-public-ip>:8080/restarthttp://<ec2-instance-public-ip>:8080/restart`
