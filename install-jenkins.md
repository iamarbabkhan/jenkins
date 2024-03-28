### Install Jenkins on ec2 aws
1. Create ec2 on aws
2. EC2 Instances - Security - edit inbound rules - all traffic - 8080
3. http://ipaddress:8080

**pre-requisites: java(jdk)**
#### INnstall Java
```
sudo apt update
sudo apt install openjdk-11-jre
java --version
```
#### Install jenkins

```
curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
```
```
sudo apt update
sudo apt install jenkins
```
#### To see jenkins default password
```
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```
